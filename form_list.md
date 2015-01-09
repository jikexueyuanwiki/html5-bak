# 新的input属性：list 

list 属性规定输入域的 datalist。datalist 是输入域的选项列表。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php" method="get">
<input list="browsers" name="browser">
<datalist id="browsers">
<option value="Internet Explorer">
<option value="Firefox">
<option value="Chrome">
<option value="Opera">
<option value="Safari">
</datalist>
<input type="submit">
</form>

<p><strong>注意:</strong> Internet Explorer 9（更早IE版本），Safari不支持 datalist 标签。</p>

</body>
</html>
```