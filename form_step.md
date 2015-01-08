# 新的input属性：step

step属性为输入域规定合法的数字间隔。

如果 step="3"，则合法的数是 -3,0,3,6 等

> 提示：step属性可以与max和min属性创建一个区域值.

> 注: step属性与以下type类型一起使用: number, range, date, datetime, datetime-local, month, time 和 week.

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">
<input type="number" name="points" step="3">
<input type="submit">
</form>

<p><strong>注意：</strong> Internet Explorer 9及更早IE版本，或Firefox不支持input标签的 step 属性。</p>

</body>
</html>
```