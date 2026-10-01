<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Abisha G · Python Full Stack Developer</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=Manrope:wght@400;600;800&family=Fira+Code:wght@400;500&display=swap" rel="stylesheet">
<style>
:root{--bg:#0d0a26;--fg:#f1efff;--mut:#b4b0e0;--acc:#f97316;--vio:#7c6cf5;--cy:#22d3ee;--glass:rgba(255,255,255,.07);--gb:rgba(255,255,255,.17);--sh:0 24px 60px rgba(0,0,0,.38);--blob:.55;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media(prefers-color-scheme:light){:root:not([data-theme="dark"]){--bg:#f1efff;--fg:#17143d;--mut:#55507f;--acc:#d9580a;--glass:rgba(255,255,255,.55);--gb:rgba(255,255,255,.95);--sh:0 24px 50px rgba(80,70,160,.2);--blob:.4}}
@media(prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0d0a26;--fg:#f1efff;--mut:#b4b0e0;--glass:rgba(255,255,255,.07);--gb:rgba(255,255,255,.17)}}
:root[data-theme="dark"]{--bg:#0d0a26;--fg:#f1efff;--mut:#b4b0e0;--glass:rgba(255,255,255,.07);--gb:rgba(255,255,255,.17)}
html{scroll-padding-top:env(safe-area-inset-top,0px);scroll-behavior:smooth}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--fg);font:400 1.05rem/1.7 Manrope,system-ui,sans-serif;-webkit-font-smoothing:antialiased;overflow-x:hidden}
main{max-width:1040px;margin:0 auto;padding:0 clamp(18px,5vw,44px)}
section{padding:clamp(64px,11vh,120px) 0;scroll-margin-top:70px}
h1,h2,h3,.big{font-family:"Instrument Serif",Georgia,serif;font-weight:400;margin:0;line-height:1.05}
h1{font-size:clamp(3.4rem,11vw,7.2rem)}
h2{font-size:clamp(2.2rem,5vw,3.4rem);margin-bottom:34px}
.big{font-size:clamp(1.6rem,3.8vw,2.6rem);line-height:1.2}
p{color:var(--mut);margin:0 0 1rem}
a{color:inherit}
a:focus-visible,button:focus-visible{outline:2px solid var(--acc);outline-offset:3px}
/* background */
.bg{position:fixed;inset:0;z-index:-1;overflow:hidden;pointer-events:none}
.bg i{position:absolute;border-radius:50%;filter:blur(80px);opacity:var(--blob);animation:fl 14s ease-in-out infinite alternate;transform:translateY(calc(var(--sy,0)*-.12px))}
.b1{width:46vmax;height:46vmax;left:-12vmax;top:-10vmax;background:var(--vio)}
.b2{width:40vmax;height:40vmax;right:-14vmax;top:30vh;background:var(--acc);animation-delay:-5s;opacity:calc(var(--blob)*.7)}
.b3{width:34vmax;height:34vmax;left:20vw;bottom:-14vmax;background:var(--cy);animation-delay:-9s;opacity:calc(var(--blob)*.55)}
@keyframes fl{to{margin:40px 0 0 50px;scale:1.12}}
.glow{position:fixed;left:0;top:0;width:340px;height:340px;margin:-170px 0 0 -170px;border-radius:50%;background:radial-gradient(circle,rgba(249,115,22,.22),transparent 65%);pointer-events:none;z-index:0;opacity:0;transition:opacity .4s}
.bar{position:fixed;top:0;left:0;right:0;height:3px;z-index:60;transform-origin:0 50%;transform:scaleX(var(--p,0));background:linear-gradient(90deg,var(--acc),var(--vio),var(--cy))}
/* glass */
.glass{position:relative;overflow:hidden;background:var(--glass);border:1px solid var(--gb);border-radius:24px;box-shadow:var(--sh),inset 0 1px 0 rgba(255,255,255,.25);-webkit-backdrop-filter:blur(18px) saturate(170%);backdrop-filter:blur(18px) saturate(170%)}
.glass::before{content:"";position:absolute;inset:0;pointer-events:none;background:radial-gradient(240px circle at var(--mx,50%) var(--my,0%),rgba(255,255,255,.2),transparent 70%);opacity:0;transition:opacity .3s}
.glass:hover::before,.glass.touch::before{opacity:1}
.tilt{transition:transform .35s cubic-bezier(.22,1,.36,1);will-change:transform}
.rip{position:relative;overflow:hidden}
.rp{position:absolute;border-radius:50%;background:rgba(255,255,255,.4);transform:scale(0);animation:rp .7s ease-out forwards;pointer-events:none}
@keyframes rp{to{transform:scale(1);opacity:0}}
/* nav */
nav{position:fixed;z-index:50;top:calc(14px + env(safe-area-inset-top,0px));left:50%;transform:translateX(-50%);display:flex;align-items:center;gap:6px;padding:7px 8px 7px 10px;border-radius:999px;width:max-content;max-width:calc(100vw - 20px)}
nav .lg{display:flex;align-items:center;gap:9px;text-decoration:none;font-weight:800;padding-right:8px}
nav svg{width:32px;height:32px;flex:none}
nav .nm{display:none}
nav a.l{padding:7px 12px;border-radius:999px;text-decoration:none;font-size:.88rem;font-weight:600;color:var(--mut);transition:background .3s,color .3s}
nav a.l:hover,nav a.l.on{background:rgba(255,255,255,.14);color:var(--fg)}
@media(min-width:620px){nav .nm{display:inline}}
@media(max-width:420px){nav a.l{padding:7px 8px;font-size:.8rem}}
/* hero */
.hero{min-height:100svh;display:grid;gap:44px;align-items:center;padding-top:110px}
@media(min-width:900px){.hero{grid-template-columns:1.1fr .9fr}}
.pill{display:inline-flex;align-items:center;gap:10px;padding:8px 16px;border-radius:999px;font-size:.88rem;font-weight:600;margin-bottom:26px}
.pill i{width:9px;height:9px;border-radius:50%;background:#34d399;box-shadow:0 0 0 0 rgba(52,211,153,.6);animation:pu 2s infinite}
@keyframes pu{70%{box-shadow:0 0 0 10px rgba(52,211,153,0)}100%{box-shadow:0 0 0 0 rgba(52,211,153,0)}}
.role{font-size:clamp(1.05rem,2.2vw,1.35rem);color:var(--mut);max-width:30ch;margin-top:24px}
.cta{display:flex;flex-wrap:wrap;gap:12px;margin-top:32px}
.btn{padding:13px 24px;border-radius:999px;font-weight:800;text-decoration:none;border:1px solid var(--gb);background:var(--glass);-webkit-backdrop-filter:blur(14px);backdrop-filter:blur(14px);transition:transform .25s,box-shadow .25s,border-color .25s}
.btn:hover{transform:translateY(-3px);border-color:var(--acc)}
.btn:active{transform:scale(.96)}
.btn.p{background:linear-gradient(135deg,var(--acc),#ff9a4d);border-color:transparent;color:#fff;box-shadow:0 10px 30px rgba(249,115,22,.4)}
.vis{position:relative;perspective:900px;padding:20px 0}
.win{padding:0;font-family:"Fira Code",monospace;font-size:clamp(.66rem,1.9vw,.84rem);line-height:1.85}
.win .tb{display:flex;gap:7px;padding:13px 16px;border-bottom:1px solid var(--gb)}
.win .tb i{width:11px;height:11px;border-radius:50%;background:#ff5f57}
.win .tb i:nth-child(2){background:#febc2e}.win .tb i:nth-child(3){background:#28c840}
.win pre{margin:0;padding:18px 20px 22px;white-space:pre;overflow:hidden}
.ln{display:block;opacity:0;transform:translateX(-10px);animation:ln .6s ease forwards}
@keyframes ln{to{opacity:1;transform:none}}
.k{color:#c792ea}.f{color:#82aaff}.s{color:#c3e88d}.c{color:var(--mut)}
@media(prefers-color-scheme:light){:root:not([data-theme="dark"]) .k{color:#7c3aed}:root:not([data-theme="dark"]) .f{color:#2563eb}:root:not([data-theme="dark"]) .s{color:#15803d}}
.chip{position:absolute;padding:9px 16px;border-radius:999px;font-weight:800;font-size:.85rem;animation:bob 5s ease-in-out infinite alternate;transform:translateY(calc(var(--sy,0)*-.05px))}
.chip.a{top:-6px;right:6%}.chip.b{bottom:18%;left:-3%;animation-delay:-2s}.chip.c{bottom:-4px;right:12%;animation-delay:-3.5s}
@keyframes bob{to{margin-top:-14px}}
/* about */
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:34px}
.stat{padding:24px 14px;text-align:center}
.stat b{display:block;font:400 clamp(2.2rem,6vw,3.6rem)/1 "Instrument Serif",serif}
.stat span{font-size:.88rem;color:var(--mut)}
.abt{padding:clamp(26px,5vw,52px)}
/* work */
.grid{display:grid;gap:20px}
@media(min-width:760px){.grid{grid-template-columns:1fr 1fr}.grid .card:first-child{grid-column:1/-1;display:grid;grid-template-columns:1.1fr 1fr;align-items:center}}
.card{display:flex;flex-direction:column;padding:14px;text-decoration:none}
.card .art{border-radius:16px;overflow:hidden;background:rgba(0,0,0,.18)}
.card .art svg{display:block;width:100%;height:auto;transition:transform .8s cubic-bezier(.22,1,.36,1)}
.card:hover .art svg{transform:scale(1.07)}
.card .tx{padding:18px 10px 10px}
.card h3{font-size:clamp(1.7rem,3vw,2.2rem)}
.tag{font-size:.8rem;font-weight:800;color:var(--acc);margin:6px 0 10px;display:block}
.go{font-weight:800;font-size:.92rem;display:inline-flex;gap:8px;transition:gap .3s}
.card:hover .go{gap:14px}
/* tools */
.mq{overflow:hidden;margin:0 -44px 28px;-webkit-mask:linear-gradient(90deg,transparent,#000 12%,#000 88%,transparent);mask:linear-gradient(90deg,transparent,#000 12%,#000 88%,transparent)}
.mq div{display:flex;gap:12px;width:max-content;animation:mq 32s linear infinite}
.mq:hover div{animation-play-state:paused}
.mq span{padding:10px 20px;border-radius:999px;font-weight:700;white-space:nowrap;background:var(--glass);border:1px solid var(--gb)}
@keyframes mq{to{transform:translateX(-50%)}}
.tools{display:grid;gap:16px;grid-template-columns:repeat(auto-fit,minmax(220px,1fr))}
.tool{padding:26px}
.tool h3{font-size:1.7rem;margin-bottom:8px}
.tool svg{width:38px;height:38px;margin-bottom:14px}
/* contact */
.end{padding:clamp(30px,6vw,70px);text-align:center}
.end .cta{justify-content:center}
footer{padding:30px 0 50px;text-align:center;color:var(--mut);font-size:.88rem}
footer svg{width:36px;height:36px;display:block;margin:0 auto 10px}
/* reveal */
.rv{opacity:0;transform:translateY(34px) scale(.97);filter:blur(8px);transition:opacity .9s ease,transform 1s cubic-bezier(.22,1,.36,1),filter .9s ease;transition-delay:var(--d,0s)}
.rv.in{opacity:1;transform:none;filter:none}
.w{display:inline-block;overflow:hidden;vertical-align:top;padding-bottom:.14em;margin-bottom:-.14em}
.w>span{display:inline-block;opacity:0;transform:translateY(105%);filter:blur(6px);transition:transform .9s cubic-bezier(.22,1,.36,1),opacity .7s ease,filter .8s ease;transition-delay:calc(var(--i)*38ms)}
.w.on>span{opacity:1;transform:none;filter:none}
.rv.in.tilt{transition:transform .35s cubic-bezier(.22,1,.36,1),opacity .9s ease,filter .9s ease;transition-delay:0s}
@media(prefers-reduced-motion:reduce){html{scroll-behavior:auto}*{animation-duration:.01s!important;animation-iteration-count:1!important}.rv,.w>span{opacity:1;transform:none;filter:none;transition:none}.ln{opacity:1;transform:none}}
</style>
</head>
<body>
<svg width="0" height="0" style="position:absolute" aria-hidden="true"><defs><linearGradient id="lg" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#f97316"/><stop offset="1" stop-color="#7c6cf5"/></linearGradient></defs><symbol id="logo" viewBox="0 0 48 48"><rect width="48" height="48" rx="14" fill="url(#lg)"/><text x="24" y="33" text-anchor="middle" font-family="Instrument Serif,Georgia,serif" font-size="26" fill="#fff">AG</text></symbol></svg>
<div class="bar"></div>
<div class="bg" aria-hidden="true"><i class="b1"></i><i class="b2"></i><i class="b3"></i></div>
<div class="glow" aria-hidden="true"></div>

<nav class="glass" aria-label="Main">
  <a class="lg" href="#top" aria-label="Abisha G home"><svg><use href="#logo"/></svg><span class="nm">Abisha G</span></a>
  <a class="l" href="#about">About</a><a class="l" href="#work">Work</a><a class="l" href="#tools">Toolbox</a><a class="l" href="#contact">Contact</a>
</nav>

<main id="top">
<section class="hero">
  <div>
    <span class="pill glass rv"><i></i>Open to full stack developer roles</span>
    <h1 data-split data-load>Abisha G</h1>
    <p class="role" data-split data-load>Python full stack developer who builds web apps you can open and use.</p>
    <div class="cta rv" style="--d:.5s">
      <a class="btn p rip" href="#work">See my work</a>
      <a class="btn rip" href="mailto:gabisha075@gmail.com">Email me</a>
    </div>
  </div>
  <div class="vis">
    <div class="glass win tilt rv" style="--d:.3s">
      <div class="tb"><i></i><i></i><i></i></div>
<pre><span class="ln c" style="animation-delay:.8s"># abisha.py</span>
<span class="ln" style="animation-delay:1.1s"><span class="k">class</span> <span class="f">Developer</span>:</span>
<span class="ln" style="animation-delay:1.4s">  stack = [<span class="s">"Django"</span>, <span class="s">"React"</span>,</span>
<span class="ln" style="animation-delay:1.7s">           <span class="s">"MySQL"</span>]</span>
<span class="ln" style="animation-delay:2s">  <span class="k">def</span> <span class="f">ship</span>(self):</span>
<span class="ln" style="animation-delay:2.3s">    <span class="k">return</span> <span class="s">"live apps"</span></span></pre>
    </div>
    <span class="chip glass a">Django</span><span class="chip glass b">React</span><span class="chip glass c">MySQL</span>
  </div>
</section>

<section id="about">
  <div class="glass abt rv">
    <div class="big" data-split>I am a BSc Computer Science graduate. I write Django back ends, shape them with React and MySQL, and ship them live.</div>
    <p style="margin:30px 0 0;max-width:60ch">Trained at Besant Technologies, then interned at Nim Technologies and Genlab IB. I like clear data models, tidy APIs and interfaces that feel quick.</p>
    <div class="stats">
      <div class="glass stat tilt"><b data-n="2">0</b><span>Internships</span></div>
      <div class="glass stat tilt"><b data-n="6">0</b><span>Projects built</span></div>
      <div class="glass stat tilt"><b data-n="1">0</b><span>Live app</span></div>
    </div>
  </div>
</section>

<section id="work">
  <h2 data-split>Selected work</h2>
  <div class="grid" id="grid"></div>
</section>

<section id="tools">
  <h2 data-split>Toolbox</h2>
  <div class="mq" aria-hidden="true"><div id="mq"></div></div>
  <div class="tools">
    <div class="glass tool tilt rv"><svg viewBox="0 0 38 38" fill="none" stroke="url(#lg)" stroke-width="2.4" stroke-linecap="round"><path d="M13 12 5 19l8 7M25 12l8 7-8 7M22 8l-6 22"/></svg><h3>Backend</h3><p>Python, Django, Flask, REST APIs</p></div>
    <div class="glass tool tilt rv" style="--d:.1s"><svg viewBox="0 0 38 38" fill="none" stroke="url(#lg)" stroke-width="2.4" stroke-linecap="round"><rect x="4" y="6" width="30" height="22" rx="4"/><path d="M13 33h12M19 28v5"/></svg><h3>Frontend</h3><p>React, Vite, JavaScript, HTML5, CSS3</p></div>
    <div class="glass tool tilt rv" style="--d:.2s"><svg viewBox="0 0 38 38" fill="none" stroke="url(#lg)" stroke-width="2.4"><ellipse cx="19" cy="9" rx="12" ry="5"/><path d="M7 9v10c0 3 5 5 12 5s12-2 12-5V9M7 19v10c0 3 5 5 12 5s12-2 12-5V19"/></svg><h3>Data</h3><p>MySQL, SQLite</p></div>
    <div class="glass tool tilt rv" style="--d:.3s"><svg viewBox="0 0 38 38" fill="none" stroke="url(#lg)" stroke-width="2.4" stroke-linecap="round"><circle cx="11" cy="8" r="4"/><circle cx="11" cy="30" r="4"/><circle cx="27" cy="16" r="4"/><path d="M11 12v14M27 20c0 6-8 4-16 6"/></svg><h3>Workflow</h3><p>Git, GitHub, MVC and MVT</p></div>
  </div>
</section>

<section id="contact">
  <div class="glass end rv">
    <div class="big" data-split>Open to full stack developer roles. Let's build something together.</div>
    <div class="cta">
      <a class="btn p rip" href="mailto:gabisha075@gmail.com">Email me</a>
      <a class="btn rip" href="https://www.linkedin.com/in/abisha-g-645010313">LinkedIn</a>
      <a class="btn rip" href="https://github.com/gabisha075-oss">GitHub</a>
    </div>
  </div>
</section>
</main>
<footer><svg><use href="#logo"/></svg>© Abisha G</footer>

<script>
(function(){
var $=function(s,c){return(c||document).querySelector(s)},$$=function(s,c){return[].slice.call((c||document).querySelectorAll(s))};
var reduce=matchMedia('(prefers-reduced-motion: reduce)').matches,root=document.documentElement;
/* project art */
function art(k,i){
  var g='<defs><linearGradient id="a'+i+'" x1="0" y1="0" x2="0" y2="1"><stop offset="0" stop-color="#f97316"/><stop offset="1" stop-color="#7c6cf5"/></linearGradient></defs>',b='',f='url(#a'+i+')';
  if(k=='bars'){[50,80,62,104,88,120].forEach(function(h,j){b+='<rect x="'+(32+j*30)+'" y="'+(132-h)+'" width="20" height="'+h+'" rx="5" fill="'+f+'"/>'});b+='<rect x="32" y="40" width="70" height="8" rx="4" fill="#fff" opacity=".5"/>'}
  if(k=='posts'){[0,1,2].forEach(function(j){b+='<circle cx="42" cy="'+(52+j*32)+'" r="10" fill="'+f+'"/><rect x="62" y="'+(44+j*32)+'" width="'+(130-j*20)+'" height="8" rx="4" fill="#fff" opacity=".6"/><rect x="62" y="'+(58+j*32)+'" width="'+(90-j*8)+'" height="6" rx="3" fill="#fff" opacity=".3"/>'})}
  if(k=='books'){[70,96,60,88,76,100,66].forEach(function(h,j){b+='<rect x="'+(34+j*26)+'" y="'+(128-h)+'" width="20" height="'+h+'" rx="3" fill="'+f+'" opacity="'+(.55+j%3*.2)+'"/>'});b+='<rect x="26" y="128" width="190" height="5" rx="2.5" fill="#fff" opacity=".5"/>'}
  if(k=='rows'){[0,1,2,3].forEach(function(j){b+='<rect x="30" y="'+(40+j*22)+'" width="180" height="16" rx="6" fill="#fff" opacity="'+(j?.16:.35)+'"/><circle cx="42" cy="'+(48+j*22)+'" r="4" fill="'+f+'"/>'})}
  if(k=='cards'){[0,1].forEach(function(j){[0,1].forEach(function(m){b+='<rect x="'+(32+m*100)+'" y="'+(40+j*46)+'" width="88" height="38" rx="9" fill="#fff" opacity=".18"/><circle cx="'+(48+m*100)+'" cy="'+(59+j*46)+'" r="8" fill="'+f+'"/><rect x="'+(62+m*100)+'" y="'+(54+j*46)+'" width="40" height="6" rx="3" fill="#fff" opacity=".6"/>'})})}
  return '<svg viewBox="0 0 240 150" role="img" aria-label="Project preview">'+g+'<rect width="240" height="150" fill="#1a1745"/><rect width="240" height="26" fill="#fff" opacity=".08"/><circle cx="14" cy="13" r="3.5" fill="#ff5f57"/><circle cx="26" cy="13" r="3.5" fill="#febc2e"/><circle cx="38" cy="13" r="3.5" fill="#28c840"/>'+b+'</svg>';
}
var P=[
["Expense Tracker","Django · MySQL · JavaScript · Live","Expense management with secure login, income and expense tracking, and PDF and Excel export.","https://expense-tracker-enx2.onrender.com","Open the live app","bars"],
["Multi-user Blog","Django · SQLite · JavaScript","A blogging platform with full CRUD, authentication and responsive templates for many authors.","https://github.com/gabisha075-oss/Multi-user-blog","View code","posts"],
["Library Management","Python · OOP","A file-based system built to practise core object-oriented design.","https://github.com/gabisha075-oss/Library-Management-System","View code","books"],
["Student Management","Python · OOP","Student records with create, read, update and delete.","https://github.com/gabisha075-oss/Student-Management-System","View code","rows"],
["Contact Management","Python · SQLite","A console app to store, search and update contacts.","https://github.com/gabisha075-oss/contact-management","View code","cards"]];
$('#grid').innerHTML=P.map(function(p,i){return '<a class="glass card tilt rip rv" style="--d:'+(i%2*.12)+'s" href="'+p[3]+'"><div class="art">'+art(p[5],i)+'</div><div class="tx"><h3>'+p[0]+'</h3><span class="tag">'+p[1]+'</span><p>'+p[2]+'</p><span class="go">'+p[4]+' <span aria-hidden="true">→</span></span></div></a>'}).join('');
var T=['Python','Django','Flask','React','Vite','JavaScript','HTML5','CSS3','MySQL','SQLite','Git','GitHub','REST APIs'];
$('#mq').innerHTML=T.concat(T).map(function(t){return'<span>'+t+'</span>'}).join('');
/* word split */
var blocks=$$('[data-split]');
blocks.forEach(function(el){var ws=el.textContent.trim().split(/\s+/);el.setAttribute('aria-label',ws.join(' '));el.textContent='';ws.forEach(function(t,i){var w=document.createElement('span');w.className='w';w.setAttribute('aria-hidden','true');w.style.setProperty('--i',i);var s=document.createElement('span');s.textContent=t;w.appendChild(s);el.appendChild(w);if(i<ws.length-1)el.appendChild(document.createTextNode(' '))})});
/* scroll */
var tick=false;
function upd(){tick=false;var vh=innerHeight,sy=scrollY,max=document.body.scrollHeight-vh;
  root.style.setProperty('--sy',sy);root.style.setProperty('--p',max>0?sy/max:0);
  blocks.forEach(function(el){var ws=$$('.w',el),n=ws.length,r=el.getBoundingClientRect(),p=el.hasAttribute('data-load')?1:Math.min(1,Math.max(0,(vh*.92-r.top)/(vh*.42+r.height*.4))),lit=reduce?n:Math.round(p*n);for(var i=0;i<n;i++)ws[i].classList.toggle('on',i<lit)})}
function req(){if(!tick){tick=true;requestAnimationFrame(upd)}}
addEventListener('scroll',req,{passive:true});addEventListener('resize',req);setTimeout(upd,60);
/* reveal, nav, counters */
var io=new IntersectionObserver(function(es){es.forEach(function(e){if(e.isIntersecting){e.target.classList.add('in');io.unobserve(e.target)}})},{threshold:.15});
$$('.rv').forEach(function(e){io.observe(e)});
var co=new IntersectionObserver(function(es){es.forEach(function(e){if(!e.isIntersecting)return;co.unobserve(e.target);var n=+e.target.dataset.n,t0=performance.now();(function f(t){var k=Math.min(1,(t-t0)/1200);e.target.textContent=Math.round(n*(1-Math.pow(1-k,3)));if(k<1)requestAnimationFrame(f)})(t0)})},{threshold:.6});
$$('[data-n]').forEach(function(e){co.observe(e)});
var no=new IntersectionObserver(function(es){es.forEach(function(e){if(e.isIntersecting)$$('nav a.l').forEach(function(a){a.classList.toggle('on',a.getAttribute('href')=='#'+e.target.id)})})},{rootMargin:'-45% 0px -50% 0px'});
$$('section[id]').forEach(function(s){no.observe(s)});
/* touch + pointer effects */
var glow=$('.glow');
addEventListener('pointermove',function(e){glow.style.opacity=1;glow.style.transform='translate('+e.clientX+'px,'+e.clientY+'px)'},{passive:true});
document.addEventListener('pointerleave',function(){glow.style.opacity=0});
$$('.glass').forEach(function(g){
  g.addEventListener('pointermove',function(e){var r=g.getBoundingClientRect(),x=(e.clientX-r.left)/r.width,y=(e.clientY-r.top)/r.height;g.style.setProperty('--mx',x*100+'%');g.style.setProperty('--my',y*100+'%');g.classList.add('touch');
    if(!reduce&&g.classList.contains('tilt')&&g.classList.contains('in')||!reduce&&g.classList.contains('tilt')&&!g.classList.contains('rv'))g.style.transform='perspective(800px) rotateX('+((.5-y)*9)+'deg) rotateY('+((x-.5)*11)+'deg) translateZ(0)'});
  function out(){g.classList.remove('touch');if(g.classList.contains('tilt'))g.style.transform=''}
  g.addEventListener('pointerleave',out);g.addEventListener('pointerup',function(e){if(e.pointerType!='mouse')setTimeout(out,350)});g.addEventListener('pointercancel',out)});
document.addEventListener('pointerdown',function(e){var t=e.target.closest&&e.target.closest('.rip');if(!t)return;var r=t.getBoundingClientRect(),d=Math.max(r.width,r.height)*2,s=document.createElement('span');s.className='rp';s.style.cssText='width:'+d+'px;height:'+d+'px;left:'+(e.clientX-r.left-d/2)+'px;top:'+(e.clientY-r.top-d/2)+'px';t.appendChild(s);setTimeout(function(){s.remove()},750)});
})();
</script>
</body>
</html>
