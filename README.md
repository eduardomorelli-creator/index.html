*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

:root{
--verde:#0f5d2f;
--verde-claro:#36b36a;
--verde-neon:#76ff7a;
--escuro:#071b12;
--texto:#263238;
--branco:#ffffff;
}

html{
scroll-behavior:smooth;
}

body{
background:
radial-gradient(circle at top,#f6fff6,#eefaf0,#ffffff);
color:var(--texto);
overflow-x:hidden;
}

/* Scrollbar */

::-webkit-scrollbar{
width:10px;
}

::-webkit-scrollbar-thumb{
background:var(--verde);
border-radius:20px;
}

/* Header */

header{
position:fixed;
top:0;
width:100%;
z-index:9999;

backdrop-filter:blur(20px);

background:
rgba(255,255,255,.75);

border-bottom:
1px solid rgba(255,255,255,.3);

box-shadow:
0 10px 30px rgba(0,0,0,.05);
}

.nav{
max-width:1300px;
margin:auto;
padding:20px 30px;

display:flex;
justify-content:space-between;
align-items:center;
}

.logo{
font-size:2rem;
font-weight:800;
color:var(--verde);
}

.logo span{
color:var(--verde-claro);
}

.nav-links{
display:flex;
gap:30px;
}

.nav-links a{
text-decoration:none;
font-weight:600;
color:#222;
transition:.3s;
}

.nav-links a:hover{
color:var(--verde);
}

/* Hero */

.hero{

min-height:100vh;

display:flex;
justify-content:center;
align-items:center;

text-align:center;

padding:120px 20px;

background:
linear-gradient(
rgba(0,0,0,.55),
rgba(0,0,0,.55)
),

url("https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1920");

background-size:cover;
background-position:center;

position:relative;

overflow:hidden;
}

.hero::before{

content:"";

position:absolute;

width:700px;
height:700px;

background:
rgba(118,255,122,.15);

border-radius:50%;

filter:blur(150px);

animation:
pulse 6s infinite;

}

@keyframes pulse{

0%{
transform:scale(1);
}

50%{
transform:scale(1.2);
}

100%{
transform:scale(1);
}

}

.hero-content{
max-width:950px;
position:relative;
z-index:2;
}

.hero h1{

font-size:5.5rem;

line-height:1.1;

font-weight:800;

color:white;

margin-bottom:20px;
}

.hero p{

font-size:1.25rem;

color:white;

opacity:.95;

margin-bottom:35px;
}/* BOTÕES */

.btn{

display:inline-block;

padding:18px 40px;

background:
linear-gradient(
45deg,
var(--verde),
var(--verde-claro)
);

color:white;

text-decoration:none;

font-weight:700;

border-radius:50px;

transition:.4s;

box-shadow:
0 15px 30px rgba(0,0,0,.25);

}

.btn:hover{

transform:
translateY(-5px)
scale(1.03);

box-shadow:
0 25px 50px rgba(0,0,0,.3);

}

/* SEÇÕES */

section{
padding:100px 8%;
}

.section-title{
text-align:center;
margin-bottom:70px;
}

.section-title h2{
font-size:3rem;
color:var(--escuro);
margin-bottom:15px;
}

.section-title p{
font-size:1.1rem;
color:#666;
max-width:700px;
margin:auto;
}

/* ESTATÍSTICAS */

.stats{

max-width:1300px;

margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(250px,1fr));

gap:25px;

}

.stat{

background:
rgba(255,255,255,.85);

backdrop-filter:
blur(20px);

padding:35px;

border-radius:25px;

text-align:center;

box-shadow:
0 15px 35px rgba(0,0,0,.08);

transition:.4s;

border:
1px solid rgba(255,255,255,.3);

}

.stat:hover{

transform:
translateY(-10px);

box-shadow:
0 25px 50px rgba(0,0,0,.12);

}

.stat h2{

font-size:3rem;

color:var(--verde);

margin-bottom:10px;

}

.stat p{
font-size:1rem;
color:#666;
}

/* CARDS */

.cards{

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(300px,1fr));

gap:30px;

}

.card{

background:white;

padding:35px;

border-radius:25px;

box-shadow:
0 15px 35px rgba(0,0,0,.08);

transition:.5s;

position:relative;

overflow:hidden;

}

.card::before{

content:"";

position:absolute;

top:0;
left:0;

width:100%;
height:5px;

background:
linear-gradient(
90deg,
var(--verde),
var(--verde-claro)
);

}

.card:hover{

transform:
translateY(-12px);

box-shadow:
0 30px 60px rgba(0,0,0,.15);

}

.card h3{

color:var(--verde);

font-size:1.4rem;

margin-bottom:15px;

}

.card p{

line-height:1.8;

color:#555;

}

/* SOBRE */

.about{

display:grid;

grid-template-columns:
1fr 1fr;

gap:50px;

align-items:center;

}

.about img{

width:100%;

border-radius:25px;

box-shadow:
0 20px 50px rgba(0,0,0,.15);

}

.about-text h3{

font-size:2rem;

color:var(--verde);

margin-bottom:20px;

}

.about-text p{

line-height:1.9;

margin-bottom:15px;

}

/* BARRA DE PROGRESSO */

.progress-container{

max-width:1000px;

margin:auto;

}

.progress{

margin-bottom:30px;

}

.progress span{

font-weight:600;

display:block;

margin-bottom:10px;

}

.progress-bar{

height:15px;

background:#ddd;

border-radius:30px;

overflow:hidden;

}

.progress-fill{

height:100%;

background:
linear-gradient(
90deg,
var(--verde),
var(--verde-neon)
);

border-radius:30px;

}/* TECNOLOGIAS */

.tech-grid{

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(280px,1fr));

gap:30px;

}

.tech-card{

background:white;

padding:35px;

border-radius:25px;

text-align:center;

box-shadow:
0 15px 35px rgba(0,0,0,.08);

transition:.4s;

}

.tech-card:hover{

transform:
translateY(-10px);

box-shadow:
0 25px 50px rgba(0,0,0,.12);

}

.tech-icon{

font-size:4rem;

margin-bottom:20px;

}

.tech-card h3{

color:var(--verde);

margin-bottom:15px;

}

/* TIMELINE */

.timeline{

max-width:1100px;

margin:auto;

position:relative;

}

.timeline::before{

content:"";

position:absolute;

left:50%;

transform:translateX(-50%);

width:4px;

height:100%;

background:
linear-gradient(
to bottom,
var(--verde),
var(--verde-claro)
);

}

.timeline-item{

width:50%;

padding:25px;

position:relative;

}

.timeline-item:nth-child(odd){

left:0;

text-align:right;

}

.timeline-item:nth-child(even){

left:50%;

}

.timeline-content{

background:white;

padding:25px;

border-radius:20px;

box-shadow:
0 10px 30px rgba(0,0,0,.08);

}

.timeline-content h3{

color:var(--verde);

margin-bottom:10px;

}

/* SUSTENTABILIDADE */

.sustentavel{

background:
linear-gradient(
135deg,
#0b3d0b,
#1b5e20
);

color:white;

position:relative;

overflow:hidden;

}

.sustentavel::before{

content:"";

position:absolute;

width:600px;

height:600px;

background:
rgba(255,255,255,.05);

border-radius:50%;

top:-200px;
right:-200px;

}

.sustentavel .section-title h2{

color:white;

}

.sustentavel .section-title p{

color:#d7ffd7;

}

/* BENEFÍCIOS */

.benefits{

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(280px,1fr));

gap:25px;

}

.benefit{

background:
rgba(255,255,255,.08);

backdrop-filter:
blur(15px);

padding:30px;

border-radius:20px;

border:
1px solid rgba(255,255,255,.15);

}

.benefit h3{

margin-bottom:15px;

font-size:1.3rem;

}

/* CTA */

.cta{

background:
linear-gradient(
135deg,
var(--verde),
var(--verde-claro)
);

text-align:center;

color:white;

padding:120px 8%;

}

.cta h2{

font-size:3.5rem;

margin-bottom:20px;

}

.cta p{

max-width:800px;

margin:auto;

font-size:1.15rem;

margin-bottom:30px;

}

/* FOOTER */

footer{

background:#05110b;

color:white;

padding:60px 8%;

}

.footer-grid{

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(250px,1fr));

gap:40px;

}

.footer-grid h3{

margin-bottom:15px;

color:var(--verde-neon);

}

.footer-grid p{

line-height:1.8;

opacity:.9;

}/* RESPONSIVIDADE */

@media(max-width:900px){

.hero h1{
font-size:3rem;
}

.hero p{
font-size:1rem;
}

.nav-links{
display:none;
}

.about{
grid-template-columns:1fr;
}

.timeline::before{
left:20px;
}

.timeline-item,
.timeline-item:nth-child(even),
.timeline-item:nth-child(odd){

width:100%;
left:0;
text-align:left;
padding-left:60px;

}

.section-title h2{
font-size:2.2rem;
}

.cta h2{
font-size:2.2rem;
}

}

/* ANIMAÇÕES */

.fade-up{
opacity:0;
transform:translateY(50px);
transition:all .8s ease;
}

.fade-up.show{
opacity:1;
transform:translateY(0);
}
