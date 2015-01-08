# 属性

ondragstar：调用了一个函数，drag(event)，它规定了被拖动的数据

setData()：设置被拖的数据类型和值

ondragover：事件规定在何处放置被拖动的数据

ondrop：当放置被拖数据时，会发生drop事件

例：

```javascript
<!DOCTYPE HTML>
<html>
<head>
<style type="text/css">
#div1 {width:488px;height:90px;padding:10px;border:1px solid #aaaaaa;}
</style>
<script type="text/javascript">
function allowDrop(ev)
{
ev.preventDefault();
}

function drag(ev)
{
ev.dataTransfer.setData("Text",ev.target.id);
}

function drop(ev)
{
ev.preventDefault();
var data=ev.dataTransfer.getData("Text");
ev.target.appendChild(document.getElementById(data));
}
</script>
</head>
<body>

<p>请把 极客学院 的图片拖放到矩形中：</p>

<div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
<br />
<img id="drag1" src="http://s1.jikexueyuan.com/current/static/images/logo.png" draggable="true" ondragstart="drag(event)" />

</body>
</html>
```