# 新的input属性：formenctype

formenctype 属性描述了表单提交到服务器的数据编码 (只对form表单中 method="post" 表单)

formenctype 属性覆盖 form 元素的 enctype 属性。

主要: 该属性与 type="submit" 和 type="image" 配合使用。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-post-enctype.php" method="post">
First name: <input type="text" name="fname"><br>
<input type="submit" value="Submit">
<input type="submit" formenctype="multipart/form-data" value="Submit as Multipart/form-data">
</form>

<p><strong>注意：</strong> Internet Explorer 9及更早IE版本不支持input标签的 formenctype 属性。</p>

</body>
</html>
```