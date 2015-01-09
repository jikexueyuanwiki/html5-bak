# 新的input属性：height 和 width 

height 和 width 属性规定用于 image 类型的 `<input>` 标签的图像高度和宽度。

> 注: height 和 width 属性只适用于 image 类型的`<input>` 标签。

> 提示:图像通常会同时指定高度和宽度属性。如果图像设置高度和宽度，图像所需的空间 在加载页时会被保留。如果没有这些属性， 浏览器不知道图像的大小，并不能预留 适当的空间。图片在加载过程中会使页面布局效果改变 （尽管图片已加载）。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">
First name: <input type="text" name="fname"><br>
Last name: <input type="text" name="lname"><br>
<input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
</form>


</body>
</html>
```