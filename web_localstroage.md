# localStroage：没有时间限制的数据存储

localStorage 方法存储的数据没有时间限制,多久以后数据都依然可用。

例：对用户访问页面的次数进行计数

```javascript
<!DOCTYPE HTML>
<html>
<body>

<script type="text/javascript">

if (localStorage.pagecount)
{
localStorage.pagecount=Number(localStorage.pagecount) +1;
}
else
{
localStorage.pagecount=1;
}
document.write("Visits: " + localStorage.pagecount + " time(s).");

</script>

<p>刷新页面会看到计数器在增长。</p>

<p>浏览器重启后，计数器会继续计数。</p>

</body>
</html>
```