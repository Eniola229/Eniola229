<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Joshua Adeyemi (Afric) — Full-Stack Developer</title>
<link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;700;800;900&family=Barlow:wght@400;500;600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --g:#22c55e;--gd:#16a34a;--gg:rgba(34,197,94,0.14);--gb:rgba(34,197,94,0.28);
  --bg:#060b14;--bg2:#0c1523;--bg3:#101e30;
  --card:#0f1c2d;--card2:#152338;
  --bd:rgba(255,255,255,0.07);--bdg:rgba(34,197,94,0.25);
  --t:#e8f2ff;--tm:#7a95b2;--td:#3f5a74;
}
html{scroll-behavior:smooth}
body{font-family:'Barlow',sans-serif;background:var(--bg);color:var(--t);overflow-x:hidden}
::-webkit-scrollbar{width:4px}::-webkit-scrollbar-track{background:var(--bg)}::-webkit-scrollbar-thumb{background:var(--gd);border-radius:2px}

/* NAV */
nav{position:fixed;top:0;left:0;right:0;z-index:100;background:rgba(6,11,20,0.92);backdrop-filter:blur(20px);border-bottom:1px solid var(--bd);display:flex;align-items:center;justify-content:space-between;padding:0 5%;height:68px}
.nav-logo{font-family:'Barlow Condensed',sans-serif;font-weight:900;font-size:17px;letter-spacing:.3px;color:var(--t);text-decoration:none}
.nav-logo .afric{color:var(--g)}
.nav-links{display:flex;gap:32px;list-style:none}
.nav-links a{font-family:'Barlow Condensed',sans-serif;font-weight:700;font-size:12px;letter-spacing:2.5px;text-transform:uppercase;color:var(--tm);text-decoration:none;transition:color .2s}
.nav-links a:hover{color:var(--g)}
.nav-cta{display:flex;gap:10px;align-items:center}
.btn-o{padding:8px 20px;border:1px solid var(--bd);background:transparent;border-radius:6px;font-family:'Barlow Condensed',sans-serif;font-weight:700;font-size:12px;letter-spacing:2px;text-transform:uppercase;cursor:pointer;color:var(--tm);text-decoration:none;transition:all .2s;display:flex;align-items:center;gap:7px}
.btn-o:hover{border-color:var(--g);color:var(--g)}
.btn-s{padding:8px 20px;background:var(--g);border:none;border-radius:6px;font-family:'Barlow Condensed',sans-serif;font-weight:700;font-size:12px;letter-spacing:2px;text-transform:uppercase;cursor:pointer;color:#000;text-decoration:none;transition:background .2s}
.btn-s:hover{background:#4ade80}

/* LABELS */
.slabel{display:flex;align-items:center;gap:12px;font-family:'Barlow Condensed',sans-serif;font-weight:700;font-size:11px;letter-spacing:3px;text-transform:uppercase;color:var(--g);margin-bottom:18px}
.slabel::before{content:'';display:block;width:26px;height:2px;background:var(--g)}

/* LIVE BADGE */
.livebadge{display:inline-flex;align-items:center;gap:7px;background:var(--gg);border:1px solid var(--bdg);color:var(--g);padding:5px 14px;border-radius:20px;font-family:'Barlow Condensed',sans-serif;font-size:11px;font-weight:700;letter-spacing:2px;text-transform:uppercase;margin-bottom:26px}
.ldot{width:7px;height:7px;background:var(--g);border-radius:50%;animation:pulse 1.5s infinite}
@keyframes pulse{0%,100%{opacity:1;box-shadow:0 0 0 0 rgba(34,197,94,.5)}50%{opacity:.7;box-shadow:0 0 0 5px rgba(34,197,94,0)}}

/* HERO */
#hero{min-height:100vh;padding:108px 5% 70px;display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center;background:var(--bg);position:relative;overflow:hidden}
#hero::before{content:'';position:absolute;top:0;left:0;right:0;bottom:0;background:radial-gradient(ellipse 55% 55% at 72% 38%,rgba(34,197,94,0.06) 0%,transparent 70%);pointer-events:none}

.hero-name{font-family:'Barlow Condensed',sans-serif;font-weight:900;line-height:.88;text-transform:uppercase;margin-bottom:24px}
.hero-name .n1{display:block;font-size:clamp(58px,6.5vw,92px);color:var(--t);animation:fu .7s both}
.hero-name .n2{display:block;font-size:clamp(58px,6.5vw,92px);color:transparent;-webkit-text-stroke:1.5px rgba(232,242,255,0.18);animation:fu .7s .15s both}
.hero-name .n3{display:block;font-size:clamp(58px,6.5vw,92px);color:var(--g);animation:fu .7s .3s both}
@keyframes fu{from{opacity:0;transform:translateY(26px)}to{opacity:1;transform:translateY(0)}}

.hero-sub{font-size:16px;line-height:1.75;color:var(--tm);max-width:400px;animation:fu .7s .45s both}
.hero-sub strong{color:var(--t)}
.hero-btns{display:flex;gap:12px;margin-top:30px;animation:fu .7s .55s both}
.hero-btns .btn-s,.hero-btns .btn-o{padding:13px 30px;font-size:13px}

/* HERO RIGHT — CYCLE BOX */
.hero-right{animation:fu .7s .2s both}
.cycle-box{background:var(--card);border:1px solid var(--bd);border-radius:16px;overflow:hidden}
.cycle-head{padding:13px 20px;border-bottom:1px solid var(--bd);display:flex;align-items:center;justify-content:space-between}
.cycle-head-l{font-family:'Barlow Condensed',sans-serif;font-size:11px;font-weight:700;letter-spacing:2.5px;text-transform:uppercase;color:var(--tm);display:flex;align-items:center;gap:8px}
.cdots{display:flex;gap:6px}
.cdot{width:8px;height:8px;border-radius:50%;background:var(--bg3);border:1px solid var(--bd);cursor:pointer;transition:background .3s,border-color .3s}
.cdot.on{background:var(--g);border-color:var(--g)}

.pslide{display:none;padding:26px 22px;animation:si .38s ease}
.pslide.on{display:block}
@keyframes si{from{opacity:0;transform:translateX(14px)}to{opacity:1;transform:translateX(0)}}

.ps-top{display:flex;align-items:center;gap:14px;margin-bottom:14px}
.ps-ico{width:50px;height:50px;border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:20px;flex-shrink:0;color:#fff}
.ps-name{font-family:'Barlow Condensed',sans-serif;font-weight:800;font-size:21px;color:var(--t);text-transform:uppercase}
.ps-url{font-size:12px;color:var(--g);margin-top:3px;display:flex;align-items:center;gap:5px}
.ps-desc{font-size:14px;color:var(--tm);line-height:1.72;margin-bottom:14px}
.ps-tags{display:flex;flex-wrap:wrap;gap:7px}
.ps-tag{font-family:'Barlow Condensed',sans-serif;font-size:11px;font-weight:700;letter-spacing:1px;text-transform:uppercase;padding:3px 10px;border:1px solid var(--bdg);color:var(--g);border-radius:4px;background:var(--gg)}
.psbar-wrap{height:2px;background:var(--bg3)}
.psbar{height:100%;background:var(--g);width:0%;transition:width .1s linear}

/* ACTIVITY */
.act-box{background:var(--card2);border:1px solid var(--bd);border-radius:12px;padding:15px 18px;margin-top:10px}
.act-hd{font-family:'Barlow Condensed',sans-serif;font-weight:700;font-size:11px;letter-spacing:2.5px;text-transform:uppercase;color:var(--tm);margin-bottom:11px;display:flex;align-items:center;gap:8px}
.act-row{font-size:13px;color:var(--tm);padding:7px 0;border-bottom:1px solid var(--bd);display:flex;align-items:center;gap:10px}
.act-row:last-child{border:none;padding-bottom:0}
.act-row i{color:var(--g);width:14px;text-align:center;font-size:13px}
.act-row strong{color:var(--t);font-weight:600}

/* FEATURES */
#features{padding:100px 5%;background:var(--bg2)}
.feat-hd{max-width:520px;margin-bottom:56px}
.feat-hd h2{font-family:'Barlow Condensed',sans-serif;font-weight:900;font-size:clamp(44px,5vw,68px);text-transform:uppercase;line-height:.92;color:var(--t)}
.fgrid{display:grid;grid-template-columns:1fr 1fr;border:1px solid var(--bd);border-radius:16px;overflow:hidden}
.fcard{padding:44px 38px;border:1px solid var(--bd);background:var(--card);transition:background .22s}
.fcard:hover{background:var(--card2)}
.fnum{font-family:'Barlow Condensed',sans-serif;font-size:11px;color:var(--td);letter-spacing:1px;margin-bottom:18px}
.fico{width:44px;height:44px;border-radius:10px;background:var(--gg);border:1px solid var(--bdg);display:flex;align-items:center;justify-content:center;margin-bottom:16px;color:var(--g);font-size:19px}
.ftitle{font-family:'Barlow Condensed',sans-serif;font-weight:800;font-size:24px;color:var(--t);margin-bottom:10px;text-transform:uppercase}
.fdesc{font-size:15px;color:var(--tm);line-height:1.75}

/* STACK */
#stack{padding:100px 5%;background:var(--bg)}
.stack-top{display:flex;justify-content:space-between;align-items:flex-end;margin-bottom:46px}
.stack-top h2{font-family:'Barlow Condensed',sans-serif;font-weight:900;font-size:clamp(44px,5vw,68px);text-transform:uppercase;line-height:.92;color:var(--t)}
.stack-top p{font-size:15px;color:var(--tm);max-width:255px;text-align:right}
.sdivider{height:1px;background:var(--bd);margin-bottom:38px}
.tgrid{border:1px solid var(--bd);border-radius:14px;overflow:hidden;background:var(--card)}
.trow{display:grid;grid-template-columns:repeat(4,1fr)}
.tcell{padding:26px 14px;text-align:center;border-right:1px solid var(--bd);border-bottom:1px solid var(--bd);transition:background .2s;cursor:default}
.trow:last-child .tcell{border-bottom:none}
.tcell:last-child{border-right:none}
.tcell:hover{background:var(--gg)}
.tcell i{font-size:26px;color:var(--tm);display:block;margin-bottom:10px;transition:color .2s}
.tcell:hover i{color:var(--g)}
.tname{font-family:'Barlow Condensed',sans-serif;font-weight:700;font-size:12px;letter-spacing:1.5px;text-transform:uppercase;color:var(--tm);transition:color .2s}
.tcell:hover .tname{color:var(--g)}

/* PROJECTS */
#projects{padding:100px 5%;background:var(--bg2)}
.proj-hd{margin-bottom:56px}
.proj-hd h2{font-family:'Barlow Condensed',sans-serif;font-weight:900;font-size:clamp(44px,5vw,68px);text-transform:uppercase;color:var(--t);line-height:.92}
.proj-hd h2 span{color:transparent;-webkit-text-stroke:1.5px rgba(232,242,255,0.14)}
.pgrid{display:grid;grid-template-columns:1fr 1fr;gap:1px;background:var(--bd);border-radius:16px;overflow:hidden}
.pcard{background:var(--card);padding:36px 32px;text-decoration:none;display:block;position:relative;border-left:3px solid transparent;transition:border-color .22s,background .22s}
.pcard:hover{background:var(--card2);border-left-color:var(--g)}
.pnum{font-family:'Barlow Condensed',sans-serif;font-size:11px;color:var(--td);letter-spacing:1.5px;text-transform:uppercase;margin-bottom:16px}
.pico-row{display:flex;align-items:center;gap:13px;margin-bottom:12px}
.pico{width:46px;height:46px;border-radius:10px;background:var(--gg);border:1px solid var(--bdg);display:flex;align-items:center;justify-content:center;color:var(--g);font-size:19px;flex-shrink:0}
.pname{font-family:'Barlow Condensed',sans-serif;font-weight:800;font-size:22px;color:var(--t);text-transform:uppercase}
.purl{font-size:12px;color:var(--g);display:flex;align-items:center;gap:5px;margin-top:2px}
.pdesc{font-size:14px;color:var(--tm);line-height:1.75;margin-bottom:16px}
.ptags{display:flex;flex-wrap:wrap;gap:7px}
.ptag{font-family:'Barlow Condensed',sans-serif;font-size:11px;font-weight:700;letter-spacing:1px;text-transform:uppercase;padding:4px 10px;border:1px solid var(--bd);color:var(--td);border-radius:4px}
.parrow{position:absolute;top:34px;right:30px;color:var(--td);font-size:13px;transition:color .2s,transform .2s}
.pcard:hover .parrow{color:var(--g);transform:translate(2px,-2px)}
.pcard.feat{grid-column:1/-1}
.pcard.feat .pdesc{max-width:560px}
.pcard.feat .pico{background:rgba(34,197,94,.2);border-color:var(--g)}
.pcard.feat .pico i{color:var(--g)}

/* CONNECT */
#connect{padding:100px 5%;background:var(--bg)}
.con-inner{display:grid;grid-template-columns:1fr 1fr;gap:80px;align-items:center}
.con-l h2{font-family:'Barlow Condensed',sans-serif;font-weight:900;font-size:clamp(44px,5vw,68px);text-transform:uppercase;line-height:.92;color:var(--t);margin-bottom:18px}
.con-l h2 span{color:var(--g)}
.con-l p{font-size:16px;color:var(--tm);line-height:1.75;margin-bottom:32px}
.clinks{display:flex;flex-direction:column;gap:10px}
.clink{display:flex;align-items:center;gap:15px;padding:15px 18px;border:1px solid var(--bd);border-radius:10px;text-decoration:none;color:var(--t);background:var(--card);transition:border-color .2s,background .2s}
.clink:hover{border-color:var(--bdg);background:var(--card2)}
.clink-ico{width:40px;height:40px;border-radius:9px;background:var(--gg);border:1px solid var(--bdg);display:flex;align-items:center;justify-content:center;color:var(--g);font-size:16px;flex-shrink:0}
.clink-lbl{font-size:11px;color:var(--td);text-transform:uppercase;letter-spacing:1.5px}
.clink-val{font-weight:600;font-size:14px;color:var(--t);margin-top:2px}
.gh-card{background:var(--card);border:1px solid var(--bd);border-radius:16px;padding:34px}
.gh-card h3{font-family:'Barlow Condensed',sans-serif;font-weight:800;font-size:21px;color:var(--t);margin-bottom:5px}
.gh-card p{font-size:14px;color:var(--tm);margin-bottom:26px;line-height:1.7}
.ghstats{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.ghs{background:var(--bg3);border:1px solid var(--bd);border-radius:10px;padding:18px;text-align:center}
.ghs-n{font-family:'Barlow Condensed',sans-serif;font-weight:900;font-size:28px;color:var(--g)}
.ghs-l{font-size:11px;color:var(--td);margin-top:4px;text-transform:uppercase;letter-spacing:1px}

/* FOOTER */
footer{background:var(--bg2);border-top:1px solid var(--bd);padding:34px 5%;display:flex;align-items:center;justify-content:space-between}
.fl{font-family:'Barlow Condensed',sans-serif;font-weight:900;font-size:17px;color:var(--t);text-decoration:none}
.fl .afric{color:var(--g)}
footer p{font-size:13px;color:var(--td)}

/* REVEAL */
.rv{opacity:0;transform:translateY(22px);transition:opacity .6s ease,transform .6s ease}
.rv.vis{opacity:1;transform:translateY(0)}

/* RESPONSIVE */
@media(max-width:960px){
  #hero{grid-template-columns:1fr}
  .hero-right{display:none}
  .fgrid,.pgrid{grid-template-columns:1fr}
  .pcard.feat{grid-column:1}
  .trow{grid-template-columns:repeat(2,1fr)}
  .con-inner{grid-template-columns:1fr;gap:40px}
  .stack-top{flex-direction:column;align-items:flex-start;gap:12px}
  .stack-top p{text-align:left}
  .nav-links{display:none}
  footer{flex-direction:column;gap:10px;text-align:center}
}
</style>
</head>
<body>

<nav>
  <a href="#" class="nav-logo">JOSHUA ADEYEMI <span class="afric">(AFRIC)</span></a>
  <ul class="nav-links">
    <li><a href="#features">What I Build</a></li>
    <li><a href="#stack">Stack</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#connect">Contact</a></li>
  </ul>
  <div class="nav-cta">
    <a href="https://github.com/Eniola229" target="_blank" class="btn-o"><i class="fa-brands fa-github"></i> GitHub</a>
    <a href="mailto:joshuaadeyemi445@gmail.com" class="btn-s">Hire Me</a>
  </div>
</nav>

<!-- HERO -->
<section id="hero">
  <div>
    <div class="livebadge"><span class="ldot"></span> Available for Work</div>
    <div class="slabel" style="margin-bottom:16px;">Full-Stack Web &amp; Mobile Developer</div>
    <div class="hero-name">
      <span class="n1">JOSHUA</span>
      <span class="n2">ADEYEMI</span>
      <span class="n3">(AFRIC)</span>
    </div>
    <p class="hero-sub">
      <strong>Laravel · React · React Native · Firebase · Tailwind.</strong><br>
      I build fintech wallets, VTU platforms, dashboards, voting systems &amp; real APIs — clean UI, scalable backend, real impact.
    </p>
    <div class="hero-btns">
      <a href="#projects" class="btn-s">View Projects</a>
      <a href="#connect" class="btn-o">Get In Touch</a>
    </div>
  </div>

  <div class="hero-right">
    <div class="cycle-box">
      <div class="cycle-head">
        <div class="cycle-head-l"><span class="ldot"></span> Live Projects</div>
        <div class="cdots" id="cdots"></div>
      </div>

      <div class="pslide on" data-i="0">
        <div class="ps-top">
          <div class="ps-ico" style="background:linear-gradient(135deg,#16a34a,#166534)"><i class="fa-solid fa-tv"></i></div>
          <div>
            <div class="ps-name">AfricTV</div>
            <div class="ps-url"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> africtv.fun</div>
          </div>
        </div>
        <p class="ps-desc">African-focused streaming platform delivering video content with modern interface and robust backend infrastructure.</p>
        <div class="ps-tags"><span class="ps-tag">React</span><span class="ps-tag">Laravel</span><span class="ps-tag">MySQL</span><span class="ps-tag">Streaming</span></div>
      </div>

      <div class="pslide" data-i="1">
        <div class="ps-top">
          <div class="ps-ico" style="background:linear-gradient(135deg,#0ea5e9,#0369a1)"><i class="fa-solid fa-cart-shopping"></i></div>
          <div>
            <div class="ps-name">OrdererWeb</div>
            <div class="ps-url"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> ordererweb.shop</div>
          </div>
        </div>
        <p class="ps-desc">Full-featured e-commerce platform with order management, product listings, and seamless payment integration.</p>
        <div class="ps-tags"><span class="ps-tag">Laravel</span><span class="ps-tag">Tailwind</span><span class="ps-tag">Paystack</span><span class="ps-tag">MySQL</span></div>
      </div>

      <div class="pslide" data-i="2">
        <div class="ps-top">
          <div class="ps-ico" style="background:linear-gradient(135deg,#7c3aed,#5b21b6)"><i class="fa-solid fa-building-columns"></i></div>
          <div>
            <div class="ps-name">LSIV</div>
            <div class="ps-url"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> lsiv.org</div>
          </div>
        </div>
        <p class="ps-desc">Professional organizational website with clean architecture, content management, and polished modern design standards.</p>
        <div class="ps-tags"><span class="ps-tag">React</span><span class="ps-tag">PHP</span><span class="ps-tag">MySQL</span><span class="ps-tag">CMS</span></div>
      </div>

      <div class="pslide" data-i="3">
        <div class="ps-top">
          <div class="ps-ico" style="background:linear-gradient(135deg,#f59e0b,#b45309)"><i class="fa-solid fa-chart-line"></i></div>
          <div>
            <div class="ps-name">TradeVista Hub</div>
            <div class="ps-url"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> tradevistahub.shop</div>
          </div>
        </div>
        <p class="ps-desc">Fintech trading hub with real-time data, portfolio tracking, and secure transaction workflows for modern traders.</p>
        <div class="ps-tags"><span class="ps-tag">React</span><span class="ps-tag">Laravel</span><span class="ps-tag">Firebase</span><span class="ps-tag">Fintech</span></div>
      </div>

      <div class="pslide" data-i="4">
        <div class="ps-top">
          <div class="ps-ico" style="background:linear-gradient(135deg,#22c55e,#15803d)"><i class="fa-solid fa-wallet"></i></div>
          <div>
            <div class="ps-name">A-Pay Wallet</div>
            <div class="ps-url"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> africicl.com.ng/a-pay</div>
          </div>
        </div>
        <p class="ps-desc">Full fintech wallet — Paystack, webhook automation, transfers, receipts &amp; admin panel. Built for scale.</p>
        <div class="ps-tags"><span class="ps-tag">Laravel</span><span class="ps-tag">Paystack</span><span class="ps-tag">Webhooks</span><span class="ps-tag">Wallet</span></div>
      </div>

      <div class="psbar-wrap"><div class="psbar" id="psbar"></div></div>
    </div>

    <div class="act-box">
      <div class="act-hd"><span class="ldot"></span> Recent Activity</div>
      <div class="act-row"><i class="fa-solid fa-bolt"></i> Launched <strong>A-Pay wallet</strong> with Paystack webhooks</div>
      <div class="act-row"><i class="fa-brands fa-react"></i> Shipped <strong>React Native app</strong> with Firebase auth</div>
      <div class="act-row"><i class="fa-solid fa-tower-broadcast"></i> Deployed <strong>VTU platform</strong> with airtime/data API</div>
    </div>
  </div>
</section>

<!-- WHAT I BUILD -->
<section id="features">
  <div class="feat-hd rv">
    <div class="slabel">What I Build</div>
    <h2>SYSTEMS THAT<br>ACTUALLY WORK</h2>
  </div>
  <div class="fgrid">
    <div class="fcard rv">
      <div class="fnum">01</div>
      <div class="fico"><i class="fa-solid fa-credit-card"></i></div>
      <div class="ftitle">Fintech &amp; Wallets</div>
      <p class="fdesc">Full wallet systems with Paystack integration, webhook automation, transaction history, and instant delivery pipelines built for scale and security.</p>
    </div>
    <div class="fcard rv">
      <div class="fnum">02</div>
      <div class="fico"><i class="fa-solid fa-gauge-high"></i></div>
      <div class="ftitle">Dashboards &amp; Web Apps</div>
      <p class="fdesc">React-powered dashboards with clean UI, real-time data feeds, admin panels, and backend APIs that handle serious traffic without breaking.</p>
    </div>
    <div class="fcard rv">
      <div class="fnum">03</div>
      <div class="fico"><i class="fa-solid fa-mobile-screen"></i></div>
      <div class="ftitle">Mobile Apps</div>
      <p class="fdesc">React Native mobile applications with Firebase or Appwrite backends, auth flows, push notifications, and production-ready UI that ships.</p>
    </div>
    <div class="fcard rv">
      <div class="fnum">04</div>
      <div class="fico"><i class="fa-solid fa-layer-group"></i></div>
      <div class="ftitle">Specialized Systems</div>
      <p class="fdesc">VTU platforms, voting systems with receipt verification, WhatsApp automation bots, and full e-commerce solutions built end-to-end.</p>
    </div>
  </div>
</section>

<!-- TECH STACK -->
<section id="stack">
  <div class="stack-top rv">
    <div>
      <div class="slabel">Tech Stack</div>
      <h2>TOOLS I<br>MASTER</h2>
    </div>
    <p>A full-stack toolkit spanning frontend, backend, mobile &amp; cloud — engineered for real-world systems.</p>
  </div>
  <div class="sdivider"></div>
  <div class="tgrid rv">
    <div class="trow">
      <div class="tcell"><i class="fa-brands fa-react"></i><div class="tname">React</div></div>
      <div class="tcell"><i class="fa-brands fa-react" style="color:#38bdf8"></i><div class="tname">React Native</div></div>
      <div class="tcell"><i class="fa-brands fa-css3-alt"></i><div class="tname">Tailwind CSS</div></div>
      <div class="tcell"><i class="fa-solid fa-swatchbook"></i><div class="tname">Material UI</div></div>
    </div>
    <div class="trow">
      <div class="tcell"><i class="fa-brands fa-laravel"></i><div class="tname">Laravel</div></div>
      <div class="tcell"><i class="fa-brands fa-php"></i><div class="tname">PHP</div></div>
      <div class="tcell"><i class="fa-brands fa-python"></i><div class="tname">Python</div></div>
      <div class="tcell"><i class="fa-solid fa-fire"></i><div class="tname">Firebase</div></div>
    </div>
    <div class="trow">
      <div class="tcell"><i class="fa-solid fa-database"></i><div class="tname">MySQL</div></div>
      <div class="tcell"><i class="fa-solid fa-leaf"></i><div class="tname">MongoDB</div></div>
      <div class="tcell"><i class="fa-solid fa-server"></i><div class="tname">Appwrite</div></div>
      <div class="tcell"><i class="fa-brands fa-docker"></i><div class="tname">Docker</div></div>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects">
  <div class="proj-hd rv">
    <div class="slabel">Portfolio</div>
    <h2>MY LIVE <span>PROJECTS</span></h2>
  </div>

  <div class="pgrid">
    <a class="pcard rv" href="https://africtv.fun" target="_blank">
      <div class="pnum">01 — STREAMING PLATFORM</div>
      <div class="pico-row">
        <div class="pico"><i class="fa-solid fa-tv"></i></div>
        <div><div class="pname">AfricTV</div><div class="purl"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> africtv.fun</div></div>
      </div>
      <p class="pdesc">African-focused streaming platform delivering rich video content with a modern, responsive interface and a robust Laravel backend built for scale.</p>
      <div class="ptags"><span class="ptag">React</span><span class="ptag">Laravel</span><span class="ptag">MySQL</span><span class="ptag">Streaming</span></div>
      <span class="parrow"><i class="fa-solid fa-arrow-up-right-from-square"></i></span>
    </a>

    <a class="pcard rv" href="https://ordererweb.shop" target="_blank">
      <div class="pnum">02 — E-COMMERCE</div>
      <div class="pico-row">
        <div class="pico"><i class="fa-solid fa-cart-shopping"></i></div>
        <div><div class="pname">OrdererWeb</div><div class="purl"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> ordererweb.shop</div></div>
      </div>
      <p class="pdesc">Full-featured e-commerce platform with product management, order tracking, and seamless Paystack payment integration for Nigerian businesses.</p>
      <div class="ptags"><span class="ptag">Laravel</span><span class="ptag">Tailwind</span><span class="ptag">Paystack</span><span class="ptag">MySQL</span></div>
      <span class="parrow"><i class="fa-solid fa-arrow-up-right-from-square"></i></span>
    </a>

    <a class="pcard rv" href="https://lsiv.org" target="_blank">
      <div class="pnum">03 — ORGANIZATION</div>
      <div class="pico-row">
        <div class="pico"><i class="fa-solid fa-building-columns"></i></div>
        <div><div class="pname">LSIV</div><div class="purl"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> lsiv.org</div></div>
      </div>
      <p class="pdesc">Professional organizational website with clean architecture, dynamic content management, and a polished modern design that communicates authority.</p>
      <div class="ptags"><span class="ptag">React</span><span class="ptag">PHP</span><span class="ptag">MySQL</span><span class="ptag">CMS</span></div>
      <span class="parrow"><i class="fa-solid fa-arrow-up-right-from-square"></i></span>
    </a>

    <a class="pcard rv" href="https://tradevistahub.shop" target="_blank">
      <div class="pnum">04 — FINTECH</div>
      <div class="pico-row">
        <div class="pico"><i class="fa-solid fa-chart-line"></i></div>
        <div><div class="pname">TradeVista Hub</div><div class="purl"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> tradevistahub.shop</div></div>
      </div>
      <p class="pdesc">Fintech trading hub with real-time market data, portfolio tracking, and secure transaction workflows designed for serious modern traders.</p>
      <div class="ptags"><span class="ptag">React</span><span class="ptag">Laravel</span><span class="ptag">Firebase</span><span class="ptag">API</span></div>
      <span class="parrow"><i class="fa-solid fa-arrow-up-right-from-square"></i></span>
    </a>

    <a class="pcard feat rv" href="https://africicl.com.ng/a-pay" target="_blank">
      <div class="pnum">05 — PAYMENT SYSTEM · FEATURED PROJECT</div>
      <div class="pico-row">
        <div class="pico"><i class="fa-solid fa-wallet"></i></div>
        <div><div class="pname">A-Pay Wallet System</div><div class="purl"><i class="fa-solid fa-arrow-up-right-from-square" style="font-size:9px"></i> africicl.com.ng/a-pay</div></div>
      </div>
      <p class="pdesc">A production-grade fintech wallet built on Paystack — with webhook automation, wallet funding, peer-to-peer transfers, transaction receipts, and a full admin dashboard. Designed for high transaction volume and built to scale without compromise.</p>
      <div class="ptags"><span class="ptag">Laravel</span><span class="ptag">React</span><span class="ptag">Paystack</span><span class="ptag">Webhooks</span><span class="ptag">MySQL</span><span class="ptag">Admin Panel</span><span class="ptag">Fintech</span></div>
      <span class="parrow"><i class="fa-solid fa-arrow-up-right-from-square"></i></span>
    </a>
  </div>
</section>

<!-- CONNECT -->
<section id="connect">
  <div class="con-inner">
    <div class="con-l rv">
      <div class="slabel">Get In Touch</div>
      <h2>LET'S BUILD<br><span>TOGETHER</span></h2>
      <p>Open to freelance projects, collaborations, and full-time opportunities. If you have a real problem that needs a serious full-stack developer — I'm your guy.</p>
      <div class="clinks">
        <a href="mailto:joshuaadeyemi445@gmail.com" class="clink">
          <div class="clink-ico"><i class="fa-solid fa-envelope"></i></div>
          <div><div class="clink-lbl">Email</div><div class="clink-val">joshuaadeyemi445@gmail.com</div></div>
        </a>
        <a href="https://www.africicl.com.ng" target="_blank" class="clink">
          <div class="clink-ico"><i class="fa-solid fa-globe"></i></div>
          <div><div class="clink-lbl">Portfolio</div><div class="clink-val">africicl.com.ng</div></div>
        </a>
        <a href="https://github.com/Eniola229" target="_blank" class="clink">
          <div class="clink-ico"><i class="fa-brands fa-github"></i></div>
          <div><div class="clink-lbl">GitHub</div><div class="clink-val">github.com/Eniola229</div></div>
        </a>
      </div>
    </div>

    <div class="rv">
      <div class="gh-card">
        <div class="slabel">GitHub</div>
        <h3>@Eniola229</h3>
        <p>Actively building and shipping real-world systems. Every repo is a live product, not a tutorial clone.</p>
        <div class="ghstats">
          <div class="ghs"><div class="ghs-n">5+</div><div class="ghs-l">Live Projects</div></div>
          <div class="ghs"><div class="ghs-n">3+</div><div class="ghs-l">Years Building</div></div>
          <div class="ghs"><div class="ghs-n" style="font-size:18px">Laravel</div><div class="ghs-l">Primary Backend</div></div>
          <div class="ghs"><div class="ghs-n" style="font-size:18px">React</div><div class="ghs-l">Primary Frontend</div></div>
        </div>
      </div>
    </div>
  </div>
</section>

<footer>
  <a href="#" class="fl">JOSHUA ADEYEMI <span class="afric">(AFRIC)</span></a>
  <p>Full-Stack Developer · Lagos, Nigeria 🇳🇬</p>
  <p>© 2025 Joshua Adeyemi</p>
</footer>

<script>
// --- ANIMATED PROJECT CYCLE ---
const slides = document.querySelectorAll('.pslide');
const bar = document.getElementById('psbar');
const dotsWrap = document.getElementById('cdots');
let cur = 0, startT = null, rafId;
const DUR = 4200;

slides.forEach((_,i) => {
  const d = document.createElement('div');
  d.className = 'cdot' + (i===0?' on':'');
  d.addEventListener('click', () => goTo(i));
  dotsWrap.appendChild(d);
});

function dots(){ return document.querySelectorAll('.cdot'); }

function goTo(idx){
  slides[cur].classList.remove('on');
  dots()[cur].classList.remove('on');
  cur = idx;
  slides[cur].classList.add('on');
  dots()[cur].classList.add('on');
  startT = null;
  cancelAnimationFrame(rafId);
  rafId = requestAnimationFrame(tick);
}

function tick(ts){
  if(!startT) startT = ts;
  const p = Math.min(((ts - startT) / DUR) * 100, 100);
  bar.style.width = p + '%';
  if(p >= 100){ goTo((cur+1) % slides.length); return; }
  rafId = requestAnimationFrame(tick);
}
rafId = requestAnimationFrame(tick);

// --- SCROLL REVEAL ---
const rvEls = document.querySelectorAll('.rv');
const obs = new IntersectionObserver((entries) => {
  entries.forEach((e, i) => {
    if(e.isIntersecting){
      setTimeout(() => e.target.classList.add('vis'), i * 70);
    }
  });
}, { threshold: 0.08 });
rvEls.forEach(el => obs.observe(el));
</script>
</body>
</html>
