# input输入类型：email

email 类型用于应该包含 e-mail 地址的输入域。

在提交表单时，会自动验证 email 域的值。

例：

```javascript
<!DOCTYPE HTML>
<html>
<body>

<form action="/example/html5/demo_form.asp" method="get">
E-mail: <input type="email" name="user_email" /><br />
<input type="submit" />
</form>

</body>
</html>
```