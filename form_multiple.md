# 新的input属性：multiple 

multiple 属性是一个 boolean 属性，规定`<input>` 元素中可选择多个值。

> 注: multiple 属性适用于以下类型的`<input>` 标签：email 和 file。: email, and file.

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">
选择图片: <input type="file" name="img" multiple>
<input type="submit">
</form>

<p>尝试选取一张或者多种图片。</p>

<p><strong>注意:</strong> Internet Explorer 9及更早IE版本不支持input标签的 multiple 属性。</p>

</body>
</html>
```