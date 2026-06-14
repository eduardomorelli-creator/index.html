<!DOCTYPE html>
<html lang="pt-BR">

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Agro Forte Sustentável</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<link rel="stylesheet" href="style.css">

</head>

<body>

<header id="header">

<nav class="nav">

<div class="logo">
Agro<span>Forte</span>
</div>

<div class="nav-links">
<a href="#inicio">Início</a>
<a href="#sobre">Sobre</a>
<a href="#tecnologia">Tecnologia</a>
<a href="#sustentabilidade">Sustentabilidade</a>
<a href="#contato">Contato</a>
</div>

</nav>

</header>

<section class="hero" id="inicio">

<div class="hero-overlay"></div>

<div class="hero-content">

<div class="badge">
🌱 Agricultura Inteligente
</div>

<h1>
Transformando o Agro com
<span>Tecnologia Sustentável</span>
</h1>

<p>
Soluções modernas para aumentar a produtividade,
preservar recursos naturais e impulsionar o futuro
do agronegócio brasileiro.
</p>

<div class="hero-buttons">

<a href="#sobre" class="btn">
Conheça Mais
</a>

<a href="#contato" class="btn btn-outline">
Fale Conosco
</a>

</div>

</div>

</section>

<section class="stats">

<div class="stat-card">
<h2 class="counter" data-target="15000">0</h2>
<p>Hectares Monitorados</p>
</div>

<div class="stat-card">
<h2 class="counter" data-target="98">0</h2>
<p>% Sustentabilidade</p>
</div>

<div class="stat-card">
<h2 class="counter" data-target="250">0</h2>
<p>Projetos Realizados</p>
</div>

<div class="stat-card">
<h2 class="counter" data-target="32">0</h2>
<p>% Economia Hídrica</p>
</div>

</section>

<section id="sobre">

<div class="section-title">
<h2>Sobre Nós</h2>
<p>
Promovemos inovação, produtividade e sustentabilidade
para um agro mais forte e eficiente.
</p>
</div>

<div class="about">

<div class="about-text">

<h3>Agro Inteligente</h3>

<p>
Utilizamos tecnologias avançadas para monitoramento,
análise de dados e otimização de recursos agrícolas.
</p>

<p>
Nossa missão é conectar inovação tecnológica com
sustentabilidade ambiental.
</p>

</div>

<div class="about-image">

<img src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1200">

</div>
*{
margin:0;
padding:0;
box-sizing:border-box;
}

:root{

--primary:#0b6b38;
--secondary:#19c37d;
--accent:#72ff9a;

--dark:#07150f;
--dark2:#0d2419;

--light:#ffffff;
--text:#263238;

--glass:rgba(255,255,255,.12);
--border:rgba(255,255,255,.18);

}

html{
scroll-behavior:smooth;
}

body{

font-family:'Poppins',sans-serif;

background:
linear-gradient(
180deg,
#f6fff8,
#ffffff
);

color:var(--text);

overflow-x:hidden;

}

/* SCROLLBAR */

::-webkit-scrollbar{
width:10px;
}

::-webkit-scrollbar-thumb{

background:
linear-gradient(
180deg,
var(--primary),
var(--secondary)
);

border-radius:20px;

}

/* HEADER */

header{

position:fixed;

top:0;
left:0;

width:100%;

z-index:9999;

backdrop-filter:blur(20px);

background:
rgba(255,255,255,.75);

border-bottom:
1px solid rgba(255,255,255,.4);

transition:.4s;

}

header.scrolled{

background:
rgba(255,255,255,.95);

box-shadow:
0 10px 35px rgba(0,0,0,.08);

}

.nav{

max-width:1400px;

margin:auto;

padding:22px 40px;

display:flex;

justify-content:space-between;
align-items:center;

}

.logo{

font-size:2rem;
font-weight:800;

color:var(--primary);

}

.logo span{

color:var(--secondary);

}

.nav-links{

display:flex;
gap:35px;

}

.nav-links a{

text-decoration:none;

font-weight:600;

color:#222;

transition:.3s;

position:relative;

}

.nav-links a::after{

content:"";

position:absolute;

bottom:-8px;
left:0;

width:0%;
height:3px;

background:var(--secondary);

transition:.3s;

border-radius:20px;

}

.nav-links a:hover::after{

width:100%;

}

.nav-links a:hover{

color:var(--primary);

}

/* HERO */

.hero{

min-height:100vh;

display:flex;

justify-content:center;
align-items:center;

text-align:center;

position:relative;

padding:120px 20px;

background:
url("https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=2000");

background-size:cover;
background-position:center;

overflow:hidden;

}

.hero-overlay{

position:absolute;

inset:0;

background:
linear-gradient(
rgba(0,0,0,.65),
rgba(0,0,0,.65)
);

}

.hero-content{

position:relative;

z-index:2;

max-width:950px;

}

.badge{

display:inline-block;

padding:12px 24px;

border-radius:50px;

margin-bottom:25px;

background:
rgba(255,255,255,.12);

backdrop-filter:blur(15px);

color:white;

font-weight:600;

border:
1px solid rgba(255,255,255,.2);

}

.hero h1{

font-size:5.8rem;

line-height:1.05;

font-weight:800;

color:white;

margin-bottom:25px;

}

.hero h1 span{

color:var(--accent);

}

.hero p{

font-size:1.25rem;

line-height:1.8;

color:white;

max-width:800px;

margin:auto;

margin-bottom:40px;

opacity:.95;

}

.hero-buttons{

display:flex;

justify-content:center;

gap:20px;

flex-wrap:wrap;

}

/* BOTÕES */

.btn{

padding:18px 42px;

border-radius:50px;

text-decoration:none;

font-weight:700;

transition:.4s;

display:inline-block;

background:
linear-gradient(
45deg,
var(--primary),
var(--secondary)
);

color:white;

box-shadow:
0 15px 35px rgba(0,0,0,.25);

}

.btn:hover{

transform:
translateY(-5px);

box-shadow:
0 25px 50px rgba(0,0,0,.35);

}

.btn-outline{

background:transparent;

border:2px solid white;

color:white;

}

.btn-outline:hover{

background:white;
color:var(--primary);

}

/* ESTATÍSTICAS */

.stats{

max-width:1400px;

margin:auto;

margin-top:-90px;

padding:0 6%;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(260px,1fr));

gap:25px;

position:relative;

z-index:5;

}

.stat-card{

padding:35px;

border-radius:25px;

background:
rgba(255,255,255,.85);

backdrop-filter:blur(20px);

box-shadow:
0 20px 50px rgba(0,0,0,.08);

text-align:center;

transition:.4s;

}

.stat-card:hover{

transform:
translateY(-10px);

}

.stat-card h2{

font-size:3rem;

color:var(--primary);

margin-bottom:10px;

}

.stat-card p{

color:#666;

font-weight:500;

}/* SEÇÕES */

section{
padding:120px 8%;
}

.section-title{
text-align:center;
margin-bottom:70px;
}

.section-title h2{

font-size:3.5rem;

color:var(--dark);

margin-bottom:20px;

font-weight:800;

}

.section-title p{

max-width:800px;

margin:auto;

line-height:1.8;

color:#666;

font-size:1.1rem;

}

/* SOBRE */

.about{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:1fr 1fr;

gap:70px;

align-items:center;

}

.about-text h3{

font-size:2.5rem;

color:var(--primary);

margin-bottom:25px;

}

.about-text p{

line-height:2;

margin-bottom:20px;

font-size:1.05rem;

}

.about-image{

position:relative;

}

.about-image img{

width:100%;

border-radius:30px;

box-shadow:
0 30px 60px rgba(0,0,0,.15);

transition:.5s;

}

.about-image img:hover{

transform:scale(1.03);

}

/* TECNOLOGIAS */

.tech-section{

background:
linear-gradient(
135deg,
#f8fff9,
#eefcf2
);

}

.tech-grid{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(320px,1fr));

gap:30px;

}

.tech-card{

padding:40px;

border-radius:30px;

background:
rgba(255,255,255,.85);

backdrop-filter:blur(20px);

border:
1px solid rgba(255,255,255,.5);

box-shadow:
0 20px 50px rgba(0,0,0,.08);

transition:.4s;

position:relative;

overflow:hidden;

}

.tech-card::before{

content:"";

position:absolute;

top:0;
left:0;

width:100%;
height:5px;

background:
linear-gradient(
90deg,
var(--primary),
var(--secondary)
);

}

.tech-card:hover{

transform:
translateY(-12px);

box-shadow:
0 35px 70px rgba(0,0,0,.12);

}

.tech-icon{

font-size:4rem;

margin-bottom:25px;

}

.tech-card h3{

font-size:1.4rem;

margin-bottom:15px;

color:var(--primary);

}

.tech-card p{

line-height:1.8;

color:#666;

}

/* BENEFÍCIOS */

.benefits{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(300px,1fr));

gap:30px;

}

.benefit{

padding:35px;

border-radius:25px;

background:white;

box-shadow:
0 20px 50px rgba(0,0,0,.08);

transition:.4s;

}

.benefit:hover{

transform:
translateY(-10px);

}

.benefit h3{

color:var(--primary);

font-size:1.4rem;

margin-bottom:15px;

}

.benefit p{

line-height:1.8;

color:#666;

}

/* SUSTENTABILIDADE */

.sustainable{

background:
linear-gradient(
135deg,
var(--dark),
var(--dark2)
);

position:relative;

overflow:hidden;

}

.sustainable::before{

content:"";

position:absolute;

width:700px;
height:700px;

background:
rgba(255,255,255,.04);

border-radius:50%;

top:-250px;
right:-250px;

}

.sustainable .section-title h2{

color:white;

}

.sustainable .section-title p{

color:#d7f8dd;

}

.sustainable-grid{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(300px,1fr));

gap:30px;

}

.sustainable-card{

padding:35px;

border-radius:25px;

background:
rgba(255,255,255,.08);

backdrop-filter:blur(15px);

border:
1px solid rgba(255,255,255,.15);

color:white;

transition:.4s;

}

.sustainable-card:hover{

transform:
translateY(-10px);

}

.sustainable-card h3{

margin-bottom:15px;

font-size:1.4rem;

color:var(--accent);

}

.sustainable-card p{

line-height:1.8;

}

/* CTA PREMIUM */

.cta{

padding:140px 8%;

text-align:center;

background:
linear-gradient(
135deg,
var(--primary),
var(--secondary)
);

color:white;

}

.cta h2{

font-size:4rem;

margin-bottom:25px;

font-weight:800;

}

.cta p{

max-width:900px;

margin:auto;

line-height:1.9;

font-size:1.15rem;

margin-bottom:40px;

}

.cta .btn{

background:white;

color:var(--primary);

}

.cta .btn:hover{

transform:
translateY(-5px)
scale(1.04);

}

/* FOOTER PREMIUM */

footer{

background:#04100b;

padding:80px 8%;

color:white;

}

.footer-grid{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(250px,1fr));

gap:40px;

}

.footer-col h3{

margin-bottom:20px;

font-size:1.3rem;

color:var(--accent);

}

.footer-col p{

line-height:1.9;

opacity:.9;

}

.footer-bottom{

text-align:center;

margin-top:60px;

padding-top:30px;

border-top:
1px solid rgba(255,255,255,.1);

opacity:.8;

}/* RESPONSIVIDADE */

@media(max-width:1100px){

.hero h1{
font-size:4rem;
}

.about{
grid-template-columns:1fr;
}

}

@media(max-width:900px){

.nav-links{
display:none;
}

.hero h1{
font-size:3rem;
}

.hero p{
font-size:1rem;
}

.section-title h2{
font-size:2.5rem;
}

.cta h2{
font-size:2.7rem;
}

.stats{
margin-top:-50px;
}

}

@media(max-width:600px){

.hero h1{
font-size:2.3rem;
}

.hero-buttons{
flex-direction:column;
align-items:center;
}

.btn{
width:100%;
max-width:300px;
}

.section-title h2{
font-size:2rem;
}

}

/* ANIMAÇÕES */

.fade-up{

opacity:0;

transform:
translateY(60px);

transition:
all .9s ease;

}

.fade-up.show{

opacity:1;

transform:
translateY(0);

}

/* EFEITO DE BRILHO */

.glow{

position:absolute;

width:500px;
height:500px;

border-radius:50%;

background:
rgba(114,255,154,.15);

filter:blur(120px);

pointer-events:none;

z-index:0;

animation:
floatGlow 8s ease-in-out infinite;

}

@keyframes floatGlow{

0%{
transform:translateY(0px);
}

50%{
transform:translateY(-30px);
}

100%{
transform:translateY(0px);
}

}
</div>

</section>
