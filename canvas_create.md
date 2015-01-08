# 创建canvas标签

创建一个Canvas标签

例：

```javascript
<!DOCTYPE HTML>
<html>
　<head>
　　<style >
　　　.canvas{
　　　　background-color:aqua;
}
　　</style>
　</head>
<body>
<canvas class=“canvas” width=“200px” height=“200px”></canvas>
</body>
</html>
```

canvas 元素本身是没有绘图能力的。所以的绘制工作必须在 JavaScript 内部完成：

```javascript
var CANVAS_WIDTH = 200 , CANVAS_HEIGHT = 200;
window.onload = function(){
　createCanvas();
}
function creatCanvas(){
　　document.body.innerHTML = “<canvas id=\”mycanvas\” width=\””+CANVAS_WIDTH+“\” height=\””+CANVAS_HEIGHT+”\”></canwas>”
}
```