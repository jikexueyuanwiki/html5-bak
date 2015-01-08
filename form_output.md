# 表单元素：output

output元素用于不同类型的输出，比如计算或脚本输出

例：

```javascript
<!DOCTYPE HTML>
<html>
<head>
<script type="text/javascript">
function resCalc()
{
numA=document.getElementById("num_a").value;
numB=document.getElementById("num_b").value;
document.getElementById("result").value=Number(numA)+Number(numB);
}
</script>
</head>
<body>
<p>使用 output 元素的简易计算器：</p>
<form onsubmit="return false">
<input id="num_a" /> +
<input id="num_b" /> =
<output id="result" onforminput="resCalc()"></output>
</form>

</body>
</html>
```