# 新的input属性：form

form 属性规定输入域所属的一个或多个表单。

> 提示:如需引用一个以上的表单，请使用空格分隔的列表。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php" id="form1">
First name: <input type="text" name="fname"><br>
<input type="submit" value="Submit">
</form>

<p> "Last name" 字段没有在form表单之内，但它也是form表单的一部分。</p>

Last name: <input type="text" name="lname" form="form1">

<p><b>注意:</b> IE不支持form属性</p>

</body>
</html>
```