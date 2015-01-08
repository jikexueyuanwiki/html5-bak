# 表单属性：novalidate

novalidate 属性的一个boolean 属性.

novalidate 属性规定在提交表单时不应该验证 form 或 input 域。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php" novalidate>
E-mail: <input type="email" name="user_email">
<input type="submit">
</form>

<p><strong>Note:</strong> The novalidate attribute of the form tag is not supported in Internet Explorer 9 and earlier versions, or in Safari.</p>

</body>
</html>
```