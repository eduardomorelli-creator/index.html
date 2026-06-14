<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Agro Forte Sustentável</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

:root{
--verde:#0b6e3c;
--verde-claro:#19c37d;
--verde-neon:#73ff9d;
--escuro:#06160f;
--texto:#263238;
--branco:#ffffff;
}

html{
scroll-behavior:smooth;
}

body{
background:#f8fffa;
color:var(--texto);
overflow-x:hidden;
}

header{
position:fixed;
top:0;
width:100%;
z-index:9999;
backdrop-filter:blur(18px);
background:rgba(255,255,255,.85);
border-bottom:1px solid rgba(255,255,255,.3);
}

.nav{
max-width:1400px;
margin:auto;
padding:20px 40px;
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

.hero{

min-height:100vh;

background:
linear-gradient(
rgba(0,0,0,.55),
rgba(0,0,0,.55)
),

url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1920');

background-size:cover;
background-position:center;

display:flex;
justify-content:center;
align-items:center;

text-align:center;

padding:120px 30px;

position:relative;
overflow:hidden;
}

.hero::before{

content:"";

position:absolute;

width:800px;
height:800px;

background:
rgba(115,255,157,.15);

border-radius:50%;

filter:blur(140px);

animation:pulse 7s infinite;
}

@keyframes pulse{

0%{
transform:scale(1);
}

50%{
transform:scale(1.15);
}

100%{
transform:scale(1);
}

}

.hero-content{
position:relative;
z-index:2;
max-width:1000px;
}

.hero-badge{

display:inline-block;

padding:12px 24px;

border-radius:50px;

background:
rgba(255,255,255,.15);

backdrop-filter:blur(10px);

color:white;

margin-bottom:25px;

font-weight:600;
}

.hero h1{

font-size:5.5rem;

line-height:1.05;

color:white;

font-weight:800;

margin-bottom:25px;
}

.hero h1 span{
color:var(--verde-neon);
}

.hero p{

font-size:1.2rem;

line-height:1.9;

color:white;

max-width:800px;

margin:auto;

margin-bottom:40px;
}

.btn{

display:inline-block;

padding:18px 40px;

border-radius:50px;

text-decoration:none;

font-weight:700;

background:
linear-gradient(
45deg,
var(--verde),
var(--verde-claro)
);

color:white;

transition:.4s;

box-shadow:
0 20px 40px rgba(0,0,0,.25);
}

.btn:hover{

transform:
translateY(-5px);

}

.stats{

max-width:1400px;

margin:auto;

padding:0 8%;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(250px,1fr));

gap:25px;

margin-top:-80px;

position:relative;

z-index:5;
}

.stat-card{

background:white;

padding:35px;

border-radius:25px;

box-shadow:
0 20px 40px rgba(0,0,0,.08);

text-align:center;
}

.stat-card h2{

font-size:3rem;

color:var(--verde);

margin-bottom:10px;
}

.stat-card p{
color:#666;
}

section{
padding:120px 8%;
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
max-width:800px;
margin:auto;
line-height:1.8;
color:#666;
}

.about{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
1fr 1fr;

gap:60px;

align-items:center;
}

.about img{

width:100%;

border-radius:30px;

box-shadow:
0 25px 50px rgba(0,0,0,.15);
}

.about-text h3{

font-size:2.2rem;

color:var(--verde);

margin-bottom:20px;
}

.about-text p{

line-height:2;

margin-bottom:15px;
}

</style>
</head>

<body>

<header>

<nav class="nav">

<div class="logo">
Agro<span>Forte</span>
</div>

<div class="nav-links">
<a href="#">Início</a>
<a href="#">Sobre</a>
<a href="#">Tecnologia</a>
<a href="#">Projetos</a>
<a href="#">Contato</a>
</div>

</nav>

</header>

<section class="hero">

<div class="hero-content">

<div class="hero-badge">
🌱 Agricultura Inteligente e Sustentável
</div>

<h1>
O Futuro do Agro
<span>Começa Agora</span>
</h1>

<p>
Unimos tecnologia, inovação e sustentabilidade para impulsionar
a produtividade no campo e construir um agronegócio mais eficiente,
rentável e ambientalmente responsável.
</p>

<a href="#" class="btn">
Conheça Nossa Solução
</a>

</div>

</section>

<section class="stats">

<div class="stat-card">
<h2>15K+</h2>
<p>Hectares Monitorados</p>
</div>

<div class="stat-card">
<h2>98%</h2>
<p>Eficiência Sustentável</p>
</div>

<div class="stat-card">
<h2>250+</h2>
<p>Projetos Executados</p>
</div>

<div class="stat-card">
<h2>32%</h2>
<p>Economia Hídrica</p>
</div>

</section>

<section>

<div class="section-title">

<h2>Quem Somos</h2>

<p>
Somos uma empresa focada em inovação agrícola,
promovendo soluções modernas para maximizar resultados
e reduzir impactos ambientais.
</p>

</div>

<div class="about">

<div class="about-text">

<h3>Transformando o Agronegócio</h3>

<p>
A Agro Forte Sustentável combina tecnologia avançada,
monitoramento inteligente e práticas sustentáveis para
aumentar a produtividade rural.
</p>

<p>
Nosso objetivo é criar um ecossistema agrícola moderno,
eficiente e preparado para os desafios do futuro.
</p>

</div>

<div>
<img src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1200">
</div>

<section>

<div class="section-title">
<h2>Tecnologias de Precisão</h2>
<p>
Aplicamos ferramentas avançadas para transformar dados em decisões estratégicas, elevando a produtividade e a sustentabilidade.
</p>
</div>

<div class="cards">

<div class="card">
<div class="icon">🚜</div>
<h3>Monitoramento Inteligente</h3>
<p>
Sensores e análises em tempo real permitem acompanhar lavouras com precisão e agir rapidamente.
</p>
</div>

<div class="card">
<div class="icon">📡</div>
<h3>Dados via Satélite</h3>
<p>
Mapeamento de áreas agrícolas para identificar oportunidades de melhoria e reduzir desperdícios.
</p>
</div>

<div class="card">
<div class="icon">🌾</div>
<h3>Gestão da Produção</h3>
<p>
Planejamento eficiente para maximizar colheitas e otimizar recursos.
</p>
</div>

</div>

</section>

<style>

.cards{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(320px,1fr));

gap:30px;

}

.card{

background:white;

padding:35px;

border-radius:30px;

box-shadow:
0 20px 50px rgba(0,0,0,.08);

transition:.4s;

}

.card:hover{

transform:
translateY(-10px);

box-shadow:
0 30px 60px rgba(0,0,0,.12);

}

.icon{

font-size:3rem;

margin-bottom:20px;

}

.card h3{

font-size:1.4rem;

color:var(--verde);

margin-bottom:15px;

}

.card p{

line-height:1.9;

color:#666;

}

.dashboard{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(280px,1fr));

gap:25px;

}

.metric{

background:
linear-gradient(
135deg,
var(--verde),
var(--verde-claro)
);

color:white;

padding:40px;

border-radius:25px;

box-shadow:
0 20px 50px rgba(0,0,0,.15);

}

.metric h2{

font-size:3rem;

margin-bottom:10px;

}

.metric p{

opacity:.95;

}

.gallery{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(300px,1fr));

gap:25px;

}

.gallery img{

width:100%;

height:280px;

object-fit:cover;

border-radius:25px;

transition:.5s;

}

.gallery img:hover{

transform:scale(1.04);

}

</style>

<section>

<div class="section-title">

<h2>Painel de Resultados</h2>

<p>
Indicadores que demonstram o impacto positivo da inovação no agronegócio moderno.
</p>

</div>

<div class="dashboard">

<div class="metric">
<h2>+42%</h2>
<p>Aumento médio de produtividade</p>
</div>

<div class="metric">
<h2>-28%</h2>
<p>Redução no consumo de água</p>
</div>

<div class="metric">
<h2>+95%</h2>
<p>Precisão nas análises agrícolas</p>
</div>

<div class="metric">
<h2>24h</h2>
<p>Monitoramento contínuo</p>
</div>

</div>

</section>

<section>

<div class="section-title">

<h2>Galeria Agro Premium</h2>

<p>
Conheça alguns dos ambientes e operações que representam o futuro do campo.
</p>

</div>

<div class="gallery">

<img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?q=80&w=1200">

<img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6?q=80&w=1200">

<img src="https://images.unsplash.com/photo-1472396961693-142e6e269027?q=80&w=1200">

<img src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1200">

<img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?q=80&w=1200">

<img src="https://images.unsplash.com/photo-1465146344425-f00d5f5c8f07?q=80&w=1200">

</div>

</section>
<style>

.projects{

max-width:1400px;
margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(350px,1fr));

gap:30px;

}

.project-card{

background:white;

border-radius:30px;

overflow:hidden;

box-shadow:
0 20px 50px rgba(0,0,0,.08);

transition:.4s;

}

.project-card:hover{

transform:
translateY(-12px);

box-shadow:
0 30px 70px rgba(0,0,0,.15);

}

.project-card img{

width:100%;
height:260px;

object-fit:cover;

}

.project-content{

padding:30px;

}

.project-content h3{

color:var(--verde);

margin-bottom:15px;

font-size:1.5rem;

}

.project-content p{

line-height:1.9;

color:#666;

}

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

border-radius:25px;

box-shadow:
0 15px 40px rgba(0,0,0,.08);

}

.timeline-content h3{

color:var(--verde);

margin-bottom:10px;

}

.sustentavel{

background:
linear-gradient(
135deg,
#062216,
#0b6e3c
);

color:white;

}

.sustentavel .section-title h2{
color:white;
}

.sustentavel .section-title p{
color:#d9ffe7;
}

.benefits{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(280px,1fr));

gap:25px;

}

.benefit{

padding:35px;

border-radius:25px;

background:
rgba(255,255,255,.08);

backdrop-filter:blur(10px);

border:
1px solid rgba(255,255,255,.15);

}

.benefit h3{

margin-bottom:15px;

color:var(--verde-neon);

}

.benefit p{

line-height:1.8;

}

</style>

<section>

<div class="section-title">

<h2>Projetos em Destaque</h2>

<p>
Casos de sucesso que demonstram como a tecnologia pode transformar a agricultura moderna.
</p>

</div>

<div class="projects">

<div class="project-card">

<img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?q=80&w=1200">

<div class="project-content">

<h3>Agricultura de Precisão</h3>

<p>
Implementação de sensores e análise de dados para aumentar produtividade e reduzir custos operacionais.
</p>

</div>

</div>

<div class="project-card">

<img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?q=80&w=1200">

<div class="project-content">

<h3>Gestão Inteligente da Água</h3>

<p>
Sistemas avançados de irrigação que otimizam recursos hídricos e reduzem desperdícios.
</p>

</div>

</div>

<div class="project-card">

<img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6?q=80&w=1200">

<div class="project-content">

<h3>Monitoramento Ambiental</h3>

<p>
Acompanhamento contínuo das condições ambientais para decisões mais eficientes.
</p>

</div>

</div>

</div>

</section>

<section>

<div class="section-title">

<h2>Nossa Evolução</h2>

<p>
Uma trajetória construída com inovação, responsabilidade e compromisso com o agronegócio.
</p>

</div>

<div class="timeline">

<div class="timeline-item">
<div class="timeline-content">
<h3>2018</h3>
<p>Fundação da Agro Forte Sustentável.</p>
</div>
</div>

<div class="timeline-item">
<div class="timeline-content">
<h3>2020</h3>
<p>Primeiros projetos de agricultura inteligente.</p>
</div>
</div>

<div class="timeline-item">
<div class="timeline-content">
<h3>2022</h3>
<p>Expansão para monitoramento agrícola regional.</p>
</div>
</div>

<div class="timeline-item">
<div class="timeline-content">
<h3>2025</h3>
<p>Integração de inteligência de dados e sustentabilidade.</p>
</div>
</div>

</div>

</section>

<section class="sustentavel">

<div class="section-title">

<h2>Sustentabilidade na Prática</h2>

<p>
Tecnologia e responsabilidade ambiental trabalhando juntas para garantir um futuro mais verde.
</p>

</div>

<div class="benefits">

<div class="benefit">
<h3>🌱 Preservação Ambiental</h3>
<p>
Redução de impactos ambientais através de práticas agrícolas sustentáveis.
</p>
</div>

<div class="benefit">
<h3>💧 Economia de Água</h3>
<p>
Uso inteligente dos recursos hídricos para maior eficiência no campo.
</p>
</div>

<div class="benefit">
<h3>♻️ Produção Responsável</h3>
<p>
Processos produtivos alinhados aos princípios de sustentabilidade.
</p>
</div>

<div class="benefit">
<h3>⚡ Eficiência Energética</h3>
<p>
Aplicação de tecnologias que reduzem desperdícios energéticos.
</p>
</div>

</div>

</section>
<style>

.testimonials{

max-width:1400px;
margin:auto;

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(320px,1fr));

gap:30px;

}

.testimonial{

background:white;

padding:35px;

border-radius:25px;

box-shadow:
0 20px 50px rgba(0,0,0,.08);

transition:.4s;

}

.testimonial:hover{

transform:
translateY(-10px);

}

.testimonial p{

line-height:1.9;

margin-bottom:20px;

color:#555;

}

.client{

display:flex;
align-items:center;
gap:15px;

}

.client img{

width:60px;
height:60px;

border-radius:50%;

object-fit:cover;

}

.client-info h4{

color:var(--verde);

}

.faq{

max-width:1100px;

margin:auto;

display:grid;

gap:20px;

}

.faq-item{

background:white;

padding:30px;

border-radius:20px;

box-shadow:
0 10px 30px rgba(0,0,0,.08);

}

.faq-item h3{

color:var(--verde);

margin-bottom:12px;

}

.faq-item p{

line-height:1.8;

color:#666;

}

.contact{

max-width:1400px;

margin:auto;

display:grid;

grid-template-columns:
1fr 1fr;

gap:40px;

}

.contact-card{

background:white;

padding:40px;

border-radius:25px;

box-shadow:
0 20px 50px rgba(0,0,0,.08);

}

.contact-card h3{

margin-bottom:20px;

color:var(--verde);

}

.contact-card p{

line-height:1.9;

margin-bottom:15px;

}

.contact-form{

display:flex;

flex-direction:column;

gap:15px;

}

.contact-form input,
.contact-form textarea{

padding:18px;

border:none;

background:#f5f7f8;

border-radius:15px;

font-size:1rem;

}

.contact-form textarea{

height:150px;

resize:none;

}

.contact-form button{

padding:18px;

border:none;

border-radius:50px;

background:
linear-gradient(
45deg,
var(--verde),
var(--verde-claro)
);

color:white;

font-weight:700;

cursor:pointer;

}

.cta{

background:
linear-gradient(
135deg,
var(--verde),
var(--verde-claro)
);

padding:140px 8%;

text-align:center;

color:white;

}

.cta h2{

font-size:4rem;

margin-bottom:25px;

}

.cta p{

max-width:800px;

margin:auto;

line-height:1.9;

margin-bottom:40px;

}

.cta a{

display:inline-block;

padding:18px 40px;

border-radius:50px;

background:white;

color:var(--verde);

font-weight:700;

text-decoration:none;

}

</style>

<section>

<div class="section-title">

<h2>O Que Nossos Parceiros Dizem</h2>

<p>
A confiança de nossos clientes é o resultado do compromisso com qualidade, inovação e resultados.
</p>

</div>

<div class="testimonials">

<div class="testimonial">

<p>
"A Agro Forte transformou completamente nossa gestão agrícola. Hoje temos mais produtividade e menor desperdício."
</p>

<div class="client">

<img src="https://randomuser.me/api/portraits/men/32.jpg">

<div class="client-info">
<h4>Carlos Mendes</h4>
<span>Produtor Rural</span>
</div>

</div>

</div>

<div class="testimonial">

<p>
"A tecnologia aplicada pela equipe trouxe decisões muito mais precisas para nossa operação."
</p>

<div class="client">

<img src="https://randomuser.me/api/portraits/women/44.jpg">

<div class="client-info">
<h4>Ana Ribeiro</h4>
<span>Engenheira Agrônoma</span>
</div>

</div>

</div>

<div class="testimonial">

<p>
"Conseguimos reduzir custos e aumentar a eficiência graças às soluções inteligentes implementadas."
</p>

<div class="client">

<img src="https://randomuser.me/api/portraits/men/51.jpg">

<div class="client-info">
<h4>Roberto Lima</h4>
<span>Empresário do Agro</span>
</div>

</div>

</div>

</div>

</section>

<section>

<div class="section-title">

<h2>Perguntas Frequentes</h2>

<p>
Tire suas dúvidas sobre nossas soluções e serviços.
</p>

</div>

<div class="faq">

<div class="faq-item">
<h3>Como funciona o monitoramento agrícola?</h3>
<p>
Utilizamos sensores, análise de dados e imagens para acompanhar as condições da produção em tempo real.
</p>
</div>

<div class="faq-item">
<h3>Quais são os benefícios da agricultura inteligente?</h3>
<p>
Maior produtividade, redução de custos, uso eficiente dos recursos e sustentabilidade.
</p>
</div>

<div class="faq-item">
<h3>As soluções servem para pequenas propriedades?</h3>
<p>
Sim. Nossos serviços podem ser adaptados para propriedades de diferentes tamanhos.
</p>
</div>

</div>

</section>

<section>

<div class="section-title">

<h2>Entre em Contato</h2>

<p>
Nossa equipe está pronta para ajudar você a levar sua produção para outro nível.
</p>

</div>

<div class="contact">

<div class="contact-card">

<h3>Informações</h3>

<p>📍 Brasil</p>

<p>📞 (00) 00000-0000</p>

<p>✉ contato@agroforte.com</p>

<p>
Atendimento especializado para produtores, cooperativas e empresas do agronegócio.
</p>

</div>

<div class="contact-card">

<form class="contact-form">

<input type="text" placeholder="Seu nome">

<input type="email" placeholder="Seu e-mail">

<textarea placeholder="Sua mensagem"></textarea>

<button type="submit">
Enviar Mensagem
</button>

</form>

</div>

</div>

</section>

<section class="cta">

<h2>
Pronto para Evoluir seu Agronegócio?
</h2>

<p>
Conheça soluções inovadoras que unem produtividade, tecnologia e sustentabilidade para o campo.
</p>

<a href="#">
Solicitar Consultoria
</a>

</section>
<style>

/* FOOTER PREMIUM */

footer{

background:#04120c;

color:white;

padding:80px 8% 30px;

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

color:var(--verde-neon);

margin-bottom:20px;

font-size:1.3rem;

}

.footer-col p,
.footer-col a{

color:rgba(255,255,255,.85);

text-decoration:none;

line-height:2;

display:block;

}

.footer-col a:hover{

color:var(--verde-neon);

}

.footer-bottom{

max-width:1400px;

margin:50px auto 0;

padding-top:25px;

border-top:
1px solid rgba(255,255,255,.1);

text-align:center;

color:rgba(255,255,255,.7);

}

/* RESPONSIVIDADE */

@media(max-width:1100px){

.about{
grid-template-columns:1fr;
}

.contact{
grid-template-columns:1fr;
}

.hero h1{
font-size:4rem;
}

.timeline::before{
left:20px;
}

.timeline-item,
.timeline-item:nth-child(odd),
.timeline-item:nth-child(even){

width:100%;

left:0;

padding-left:60px;

text-align:left;

}

}

@media(max-width:900px){

.nav{
padding:20px;
}

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
font-size:2.3rem;
}

.cta h2{
font-size:2.6rem;
}

}

@media(max-width:600px){

.hero{
padding:120px 20px;
}

.hero h1{
font-size:2.2rem;
}

.btn{
display:block;
width:100%;
}

.section-title h2{
font-size:2rem;
}

.cta h2{
font-size:2rem;
}

}

/* EFEITOS EXTRAS */

.card,
.project-card,
.testimonial,
.stat-card,
.contact-card{

transition:.4s;

}

.card:hover,
.project-card:hover,
.testimonial:hover,
.contact-card:hover{

transform:
translateY(-10px);

}

html{
scroll-behavior:smooth;
}

</style>

<footer>

<div class="footer-grid">

<div class="footer-col">

<h3>Agro Forte</h3>

<p>
Transformando o agronegócio através da tecnologia,
inovação e sustentabilidade.
</p>

</div>

<div class="footer-col">

<h3>Navegação</h3>

<a href="#">Início</a>
<a href="#">Sobre</a>
<a href="#">Tecnologias</a>
<a href="#">Projetos</a>
<a href="#">Contato</a>

</div>

<div class="footer-col">

<h3>Serviços</h3>

<a href="#">Agricultura Inteligente</a>
<a href="#">Monitoramento</a>
<a href="#">Consultoria</a>
<a href="#">Sustentabilidade</a>

</div>

<div class="footer-col">

<h3>Contato</h3>

<p>📍 Brasil</p>
<p>📞 (00) 00000-0000</p>
<p>✉ contato@agroforte.com</p>

</div>

</div>

<div class="footer-bottom">

© 2026 Agro Forte Sustentável.
Todos os direitos reservados.

</div>

</footer>

</body>
</html>
</div>

</section>
