<!DOCTYPE html>
<html>
<body>

<canvas id="myCanvas" width="350" height="350" style="border:5px solid black;">
Your browser does not support the HTML canvas tag.</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var n=12;
for (let i = 1; i < n; i++) {
ctx.moveTo(i/n*(c.width),0);
ctx.lineTo(i/n*(c.width),(c.height));

ctx.moveTo(0,i/n*(c.width));
ctx.lineTo((c.height),i/n*(c.width));
ctx.stroke();
}

</script>

</body>
</html>

