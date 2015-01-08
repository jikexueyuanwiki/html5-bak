# 接收 Server-Sent 事件通知

EventSource 对象用于接收服务器发送事件通知

例：

创建一个新的 EventSource 对象，然后规定发送更新的页面的 URL（本例中是 "demo_sse.php"）

每接收到一次更新，就会发生 onmessage 事件

当 onmessage 事件发生时，把已接收的数据推入 id 为 "result" 的元素中

```javascript
<!DOCTYPE html>
<html>
<body>
<h1>获得服务器更新</h1>
<div id="result"></div>

<script>
if(typeof(EventSource)!=="undefined")
{
var source=new EventSource("/example/html5/demo_sse.php");
source.onmessage=function(event)
{
document.getElementById("result").innerHTML+=event.data + "<br />";
};
}
else
{
document.getElementById("result").innerHTML="Sorry, your browser does not support server-sent events...";
}
</script>

</body>
</html>
```