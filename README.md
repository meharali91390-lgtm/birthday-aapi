<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Aapi 🎂</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:linear-gradient(135deg,#ff9a9e,#fad0c4,#fbc2eb);
overflow:hidden;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
}

.container{
text-align:center;
color:white;
animation:fadeIn 2s ease;
padding:20px;
}

h1{
font-size:42px;
text-shadow:2px 2px 10px rgba(0,0,0,.3);
}

p{
font-size:22px;
margin-top:20px;
line-height:1.8;
}

button{
margin-top:30px;
padding:15px 35px;
font-size:20px;
border:none;
border-radius:50px;
background:white;
color:#ff4d6d;
cursor:pointer;
font-weight:bold;
transition:.3s;
}

button:hover{
transform:scale(1.08);
}

#message{
display:none;
margin-top:30px;
font-size:24px;
animation:fadeIn 2s;
}

@keyframes fadeIn{
from{
opacity:0;
transform:translateY(30px);
}
to{
opacity:1;
transform:translateY(0);
}
}

.balloon{
position:absolute;
bottom:-150px;
width:60px;
animation:float 10s linear infinite;
}

@keyframes float{
0%{
transform:translateY(0);
}
100%{
transform:translateY(-120vh);
}
}
</style>
</<audio id="bgMusic" autoplay loop>
  <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_c8b2c8f6d7.mp3?filename=gentle-piano-ambient-110624.mp3" type="audio/mpeg">
</audio>

<script>
function showWish(){
    document.getElementById("message").style.display="block";
    document.getElementById("bgMusic").play();

    for(let i=0;i<25;i++){
        let b=document.createElement("div");
        b.className="balloon";
        b.innerHTML="🎈";
        b.style.left=Math.random()*100+"vw";
        b.style.fontSize=(30+Math.random()*40)+"px";
        b.style.animationDuration=(6+Math.random()*5)+"s";
        document.body.appendChild(b);
    }
}
</script>

</body>
</html>
