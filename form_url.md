# input输入类型：url

url 类型用于应该包含 URL 地址的输入域。

在提交表单时，会自动验证 url 域的值。

例：

```javascript
<!DOCTYPE HTML>
<html>
<body>

<form action="/example/html5/demo_form.asp" method="get">
Homepage: <input type="url" name="user_url" /><br />
<input type="submit" />
</form>

</body>
</html>
```