# 检测 Server-Sent 事件支持

实例：使用一段额外的代码来检测服务器发送事件的浏览器支持情况：

```javascript
if(typeof(EventSource)!=="undefined")
{
// Yes! Server-sent events support!
// Some code.....
}
else
{
// Sorry! No server-sent events support..
}
```