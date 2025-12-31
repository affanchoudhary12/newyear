# <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy New Year 2026</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box}
html,body{height:100%;font-family:'Poppins',sans-serif;overflow:hidden}

/* animated gradient background */
body{
background:linear-gradient(270deg,#0f2027,#203a43,#2c5364,#000);
background-size:800% 800%;
animation:bgMove 18s ease infinite;
color:white;
}

@keyframes bgMove{
0%{background-position:0% 50%}
50%{background-position:100% 50%}
100%{background-position:0% 50%}
}

/* floating particles */
.particle{
position:absolute;
width:6px;
height:6px;
background:rgba(255,255,255,0.4);
border-radius:50%;
animation:float 10s linear infinite;
}
@keyframes float{
from{transform:translateY(110vh)}
to{transform:translateY(-10vh)}
}

/* sections */
section{
height:100vh;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
padding:40px;
}

.card{
background:rgba(255,255,255,0.08);
backdrop-filter:blur(14px);
border-radius:30px;
padding:60px;
max-width:900px;
animation:fadeUp 1.8s ease;
}

@keyframes fadeUp{
from{opacity:0;transform:translateY(60px)}
to{opacity:1;transform:translateY(0)}
}

h1{font-size:52px;letter-spacing:2px}
h2{font-size:34px;margin-bottom:20px}
p{font-size:18px;line-height:1.9;opacity:0.92}

/* button */
.btn{
margin-top:35px;
padding:14px 40px;
border-radius:40px;
border:1px solid white;
background:transparent;
color:white;
font-size:16px;
cursor:pointer;
transition:0.4s;
}
.btn:hover{
background:white;
color:black;
}

/* glow on click */
.glow{
animation:glow 1s ease;
}
@keyframes glow{
0%{box-shadow:0 0 0px #00fff0}
100%{box-shadow:0 0 35px #00fff0}
}

/* signature */
.signature{
text-shadow:0 0 25px #00fff0;
animation:pulse 2s infinite alternate;
}
@keyframes pulse{
from{text-shadow:0 0 10px #00fff0}
to{text-shadow:0 0 30px #00fff0}
}
</style>
</head>

<body>

<!-- particles -->
<script>
for(let i=0;i<40;i++){
let p=document.createElement("div");
p.className="particle";
p.style.left=Math.random()*100+"vw";
p.style.animationDuration=5+Math.random()*10+"s";
document.body.appendChild(p);
}
</script>

<!-- SECTION 1 -->
<section id="s1">
<div class="card">
<h1>✨ Happy New Year 2026 ✨</h1>
<p>
Ek naya saal, nayi energy aur<br>
ek strong team ke saath aage badhne ka waqt.
</p>
<button class="btn" onclick="go('s2',this)">Click to Continue ↓</button>
</div>
</section>

<!-- SECTION 2 -->
<section id="s2">
<div class="card">
<h2>Leadership & Team</h2>
<p>
Is naye saal ki shuruaat karte hue<br><br>

<b>Respected Manager – Mr. Ratan Sir</b><br>
<b>Coordinator – Mr. Sandeep</b><br><br>

aur humare sabhi talented engineers ko
dil se New Year wishes.
</p>

<p>
Aap sabki mehnat, dedication aur teamwork
hi humari asli strength hai.
</p>

<button class="btn" onclick="go('s3',this)">Next ↓</button>
</div>
</section>

<!-- SECTION 3 -->
<section id="s3">
<div class="card">
<h2>Gratitude & Vision</h2>
<p>
Aise professional aur supportive environment ka hissa banna
truly motivating hai.
</p>

<p>
Ye saal naye goals, better learning
aur collective success lekar aaye — yahi wish hai.
</p>

<button class="btn" onclick="go('s4',this)">Final ↓</button>
</div>
</section>

<!-- SECTION 4 -->
<section id="s4">
<div class="card glow">
<h2 class="signature">Crafted with dedication ✨</h2>
<p>
Sabhi ko ek positive, productive aur successful
New Year ki hardik shubhkamnayein.
</p>
<br>
<h3>— Mohd Affan</h3>
</div>
</section>

<script>
function go(id,btn){
btn.parentElement.classList.add("glow");
document.getElementById(id).scrollIntoView({behavior:"smooth"});
}
</script>

</body>
</html>
newyear
