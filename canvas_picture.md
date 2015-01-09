# 利用Canvas标签绘制图形

API文档：developer.mozilia.org

例：

```javascript
var CANVAS_WIDTH = 200 , CANVAS_HEIGHT = 200;
var mycanvas,context;

window.onload = function(){
　createCanvas();
　drawRect()
}

function creatCanvas(){
　　document.body.innerHTML = “<canvas id=\”mycanvas\” width=\””+CANVAS_WIDTH+“\” height=\””+CANVAS_HEIGHT+”\”></canwas>”
　　mycanvas = document.getElementById(“mycanvas”);
　　context = mycanvas.getContext(“2d”);
}
function drawRect(){
　　context.fillRect(0,0,200,200);
}
```