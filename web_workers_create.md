# Web Workers的创建

## 检测浏览器支持

```javascript
if(typeof(Worker)!=="undefined")
  {
  // Yes! Web worker support!
  // Some code.....
  }
else
  {
  // Sorry! No Web Worker support..
  }
```

## 方法

postMessage() 用于向HTML页面传回一段消息

terminate（） 终止web worker，并释放浏览器/计算机资源

## 创建Web Workers

创建webworker文件

例：创建count.js脚本，用于计数

```javascript
var countNum = 0;
function count(){
　postMessage(countNum);
　countNum++;
　setTimeout(count,1000);
}
```

创建脚本index.js，用于处理count.js所返回的内容，并更新主UI

```javascript
var  numDiv
window.onload = function(){
　numDiv = document.getElementById(“numDiv”);
　var work = new Worker(“count.js");
　work.onmessage = function(e){
　　numDiv.innerHTML = e.data;
　}
}
```

在HTML文件中引入

```javascript
<!DOCTYPE html>
<html>
<head>
　<script src=“index.js”></script>
</head>
<body>
　<div id=“numDiv”>0</div>
</body>
</html>
```