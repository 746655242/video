# video
HTML5 video网页播放器 适用ie11及以上浏览器,后续兼容更多浏览器
#使用方法
```html
<link href="css/video-js-min.css" rel="stylesheet">

<div style="width:600px" >
    <video id="my-video">
         <source src="oceans.mp4" type="video/mp4">     
         <p class="vjs-no-js">
         	您浏览器不支持播放器，请升级！
         </p>
    </video>
	</div>

<script src="js/video-min.js"></script>

<script>
var Options={
	"autoplay":false,//是否自动播放
	"endedfn":function(){//结束回调
		console.log('谢谢观看');	
	},
	"nextfn":function(){//下个事件
		console.log('下个事件');	
	},
	"volume":50,//默认音量（1-100）
	"currentTime":0,//播放起点，单位为秒
}
var Video=new video();	
Video.init('my-video',Options); //init(id,Options);id为必填，Options为选填

```

#demo地址
http://h.hemaj.com/html/video/video.html
