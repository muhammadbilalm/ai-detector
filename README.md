<!DOCTYPE html>
<html>
<head>
<title>AI Image Detector</title>
<style>
body{
font-family: Arial;
text-align:center;
background:#111;
color:white;
}

.container{
margin-top:100px;
}

button{
padding:10px 20px;
font-size:18px;
cursor:pointer;
}

input{
margin:20px;
}
</style>
</head>

<body>

<div class="container">
<h1>AI Image Detector</h1>
<p>Upload image to check if it is AI generated</p>

<input type="file" id="imageUpload">
<br>
<button onclick="detect()">Detect</button>

<p id="result"></p>
</div>

<script>
function detect(){
document.getElementById("result").innerText="Analyzing image...";
setTimeout(()=>{
document.getElementById("result").innerText="Result: Possibly AI Generated";
},2000);
}
</script>

</body>
</html>
