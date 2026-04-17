<svg fill="none" viewBox="0 0 860 420" width="860" height="420" xmlns="http://www.w3.org/2000/svg">
<foreignObject width="100%" height="100%">
<div xmlns="http://www.w3.org/1999/xhtml">
<style>
*{box-sizing:border-box;margin:0;padding:0}
.wrap{
  width:860px;height:420px;
  background:#060b14;
  font-family:ui-monospace,SFMono-Regular,Menlo,monospace;
  position:relative;overflow:hidden;
  border-radius:12px;
}
.glow{
  position:absolute;top:-60px;right:-60px;
  width:380px;height:380px;
  background:radial-gradient(circle,rgba(34,197,94,0.13) 0%,transparent 70%);
  pointer-events:none;
}
.glow2{
  position:absolute;bottom:-80px;left:200px;
  width:300px;height:300px;
  background:radial-gradient(circle,rgba(34,197,94,0.06) 0%,transparent 70%);
  pointer-events:none;
}
.content{padding:46px 52px;position:relative;z-index:1}

/* LIVE BADGE */
.badge{
  display:inline-flex;align-items:center;gap:8px;
  background:rgba(34,197,94,0.12);
  border:1px solid rgba(34,197,94,0.3);
  color:#22c55e;padding:5px 14px;border-radius:20px;
  font-size:10px;font-weight:700;letter-spacing:2.5px;
  text-transform:uppercase;margin-bottom:22px;
}
.dot{
  width:6px;height:6px;border-radius:50%;
  background:#22c55e;flex-shrink:0;
  animation:pulse 1.6s ease-in-out infinite;
}
@keyframes pulse{
  0%,100%{box-shadow:0 0 0 0 rgba(34,197,94,.5)}
  50%{box-shadow:0 0 0 5px rgba(34,197,94,0)}
}

/* NAME */
.label{
  font-size:10px;font-weight:700;letter-spacing:3px;
  text-transform:uppercase;color:#22c55e;
  display:flex;align-items:center;gap:10px;margin-bottom:14px;
}
.label::before{content:'';display:block;width:22px;height:2px;background:#22c55e}
.name{line-height:0.88;text-transform:uppercase;margin-bottom:18px}
.n1{display:block;font-size:78px;font-weight:900;color:#e8f2ff;font-family:ui-monospace,monospace;letter-spacing:-2px;animation:slideUp .6s ease both}
.n2{display:block;font-size:78px;font-weight:900;color:transparent;font-family:ui-monospace,monospace;letter-spacing:-2px;
  -webkit-text-stroke:1.5px rgba(232,242,255,0.16);animation:slideUp .6s .12s ease both}
.n3{display:block;font-size:78px;font-weight:900;color:#22c55e;font-family:ui-monospace,monospace;letter-spacing:-2px;animation:slideUp .6s .24s ease both}
@keyframes slideUp{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:translateY(0)}}

.sub{font-size:13px;color:#7a95b2;line-height:1.7;margin-bottom:24px;max-width:360px;animation:slideUp .6s .38s ease both}
.sub strong{color:#e8f2ff}

/* TAGS ROW */
.tags{display:flex;gap:8px;flex-wrap:wrap;animation:slideUp .6s .46s ease both}
.tag{
  font-size:9px;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;
  padding:4px 11px;border:1px solid rgba(34,197,94,0.3);
  color:#22c55e;border-radius:4px;background:rgba(34,197,94,0.1);
}

/* RIGHT PANEL */
.panel{
  position:absolute;right:40px;top:38px;
  width:265px;
  background:#0f1c2d;
  border:1px solid rgba(255,255,255,0.07);
  border-radius:14px;overflow:hidden;
  animation:slideUp .6s .2s ease both;
}
.panel-head{
  padding:11px 16px;border-bottom:1px solid rgba(255,255,255,0.07);
  display:flex;align-items:center;gap:8px;
  font-size:9px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:#7a95b2;
}
.panel-body{padding:16px}
.stack-row{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:12px}
.sitem{
  font-size:9px;font-weight:700;letter-spacing:1px;text-transform:uppercase;
  padding:3px 9px;border:1px solid rgba(34,197,94,0.2);
  color:#22c55e;border-radius:3px;background:rgba(34,197,94,0.08);
}
.stat-row{display:flex;gap:8px;margin-top:4px}
.stat{
  flex:1;background:#101e30;border:1px solid rgba(255,255,255,0.06);
  border-radius:8px;padding:12px 10px;text-align:center;
}
.stat-n{font-size:22px;font-weight:900;color:#22c55e;line-height:1;font-family:ui-monospace,monospace}
.stat-l{font-size:8px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:#3f5a74;margin-top:4px}
.divider{height:1px;background:rgba(255,255,255,0.06);margin:12px 0}
.act-item{display:flex;align-items:flex-start;gap:8px;padding:5px 0;border-bottom:1px solid rgba(255,255,255,0.05);font-size:10px;color:#7a95b2;line-height:1.4}
.act-item:last-child{border:none}
.act-dot{width:5px;height:5px;border-radius:50%;background:#22c55e;flex-shrink:0;margin-top:4px}
.act-item strong{color:#e8f2ff}

/* BOTTOM BAR */
.bar{
  position:absolute;bottom:0;left:0;right:0;height:2px;
  background:linear-gradient(90deg,#22c55e,#16a34a,transparent);
  animation:barIn 1.2s ease both;
}
@keyframes barIn{from{width:0}to{width:100%}}
</style>
<div class="wrap">
  <div class="glow"></div>
  <div class="glow2"></div>

  <div class="content">
    <div class="badge"><span class="dot"></span> Available for Work</div>
    <div class="label">Full-Stack Web &amp; Mobile Developer</div>
    <div class="name">
      <span class="n1">JOSHUA</span>
      <span class="n2">ADEYEMI</span>
      <span class="n3">(AFRIC)</span>
    </div>
    <p class="sub"><strong>PHP · Laravel · React · React Native · Tailwind</strong><br/>Fintech wallets · VTU platforms · Dashboards · E-commerce · CRM · Voting systems</p>
    <div class="tags">
      <span class="tag">Laravel</span>
      <span class="tag">React</span>
      <span class="tag">React Native</span>
      <span class="tag">Firebase</span>
      <span class="tag">MySQL</span>
      <span class="tag">Paystack</span>
    </div>
  </div>

  <!-- RIGHT PANEL -->
  <div class="panel">
    <div class="panel-head"><span class="dot"></span> Quick Stats</div>
    <div class="panel-body">
      <div class="stack-row">
        <span class="sitem">PHP</span>
        <span class="sitem">Laravel</span>
        <span class="sitem">React</span>
        <span class="sitem">MySQL</span>
        <span class="sitem">Firebase</span>
        <span class="sitem">Docker</span>
      </div>
      <div class="stat-row">
        <div class="stat"><div class="stat-n">5+</div><div class="stat-l">Projects</div></div>
        <div class="stat"><div class="stat-n">3+</div><div class="stat-l">Yrs Exp</div></div>
      </div>
      <div class="divider"></div>
      <div class="act-item"><span class="act-dot"></span><span>Launched <strong>A-Pay</strong> fintech wallet</span></div>
      <div class="act-item"><span class="act-dot"></span><span>Shipped <strong>React Native</strong> app</span></div>
      <div class="act-item"><span class="act-dot"></span><span>Deployed <strong>VTU platform</strong></span></div>
    </div>
  </div>

  <div class="bar"></div>
</div>
</div>
</foreignObject>
</svg>
