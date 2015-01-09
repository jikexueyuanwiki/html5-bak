# 新的input属性：formaction

The formaction 属性用于描述表单提交的URL地址，会覆盖<form> 元素中的action属性.

> 注: The formaction 属性用于 type="submit" 和 type="image".

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">
First name: <input type="text" name="fname"><br>
Last name: <input type="text" name="lname"><br>
<input type="submit" value="Submit"><br>
<input type="submit" formaction="demo-admin.php" value="Submit as admin">
</form>
<p><strong>注意：</strong> Internet Explorer 9及更早IE版本不支持input标签的 formaction 属性。</p>

</body>
</html>
```
