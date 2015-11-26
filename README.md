# Lab-1
<!DOCTYPE HTML>
<html>
<head>
<style>
.td {
width: 210px;
height: 60px;
font-size: 36px;
text-align: center;
position: absolute;
}
#area {
position: relative;
height: 500px;
background-color: #00FFFF;
}

#answer {
font-size: 36px;
color: blue;
}

#chisla {
font-size: 24px;
color: maroon;
}
</style>
</head>

<body>


<div id="area">

<input placeholder="Введите заряд 1" id="td11">
<input placeholder="Введите заряд 2" id="td12">
<input placeholder="Введите расстояние" id="td21">
<input placeholder="Введите коэффициент" id="td22">
<input type="button" 
          value="Вычислить" onclick="MyFunction()" style="position: absolute; top:40px; left: 10px; width: 120px; height: 50px; background-color: silver;">	

<span style="position: absolute; top:100px; left:10px;" id = "answer"> Ответ </span>
</div>
<div>

</div>
</body>
</html>

<script>
function MyFunction() {
var q1, q2, r, k, F;
q1 = parseInt( document.getElementById("td11").value );
q2 = parseInt( document.getElementById("td12").value );
r = parseInt( document.getElementById("td21").value );
k = parseInt( document.getElementById("td22").value );
F = k*(q1*q2/(r*r));
document.getElementById("answer").innerHTML = 
String( F );

}

</script>
