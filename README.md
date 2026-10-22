# Stammt-der-Mensch-vom-Affen-ab<!doctype html>
<html lang="de">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Fallakte Mensch und Affe</title>
<style>
:root{--navy:#14213D;--coral:#E4572E;--amber:#F2A900;--teal:#12907F;--violet:#6C4AB6;--green:#3E8E41;--paper:#FFFDF7;--ink:#1b2430;--mute:#5b6b78;--card:#fff;--line:#e3dccb}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{margin:0;font-family:Inter,"Segoe UI",system-ui,Helvetica,Arial,sans-serif;background:var(--paper);color:var(--ink);line-height:1.5;font-size:16px}
button{font:inherit;cursor:pointer}
.wrap{max-width:1080px;margin:0 auto;padding:0 18px}
/* Kopf */
.hero{background:linear-gradient(135deg,#14213D 0%,#1f3560 100%);color:#fff;position:relative;overflow:hidden;padding:26px 0 30px}
.hero:before{content:"";position:absolute;right:-90px;top:-110px;width:360px;height:360px;border-radius:50%;background:var(--amber);opacity:.16}
.hero:after{content:"";position:absolute;left:-60px;bottom:-130px;width:300px;height:300px;border-radius:50%;background:var(--teal);opacity:.18}
.hero .wrap{position:relative;z-index:1}
.tag{display:inline-block;background:var(--amber);color:var(--navy);font-weight:800;font-size:12px;letter-spacing:.12em;padding:3px 10px;border-radius:4px}
h1{font-size:clamp(28px,5vw,46px);line-height:1.08;margin:10px 0 6px;font-weight:800}
.lead{font-size:18px;opacity:.9;max-width:640px;margin:0 0 16px}
.top{display:flex;gap:12px;flex-wrap:wrap;align-items:center;margin-top:14px}
.top input{padding:9px 12px;border-radius:8px;border:2px solid rgba(255,255,255,.35);background:rgba(255,255,255,.1);color:#fff;font:inherit;min-width:210px}
.top input::placeholder{color:rgba(255,255,255,.6)}
.bar{flex:1;min-width:220px;max-width:420px}
.bar small{display:block;font-size:12px;opacity:.85;margin-bottom:3px}
.track{height:12px;border-radius:8px;background:rgba(255,255,255,.2);overflow:hidden}
.fill{height:100%;width:0;background:linear-gradient(90deg,var(--amber),#ffd36a);transition:width .5s}
.ghost{background:transparent;color:#fff;border:2px solid rgba(255,255,255,.4);border-radius:8px;padding:7px 12px;font-size:14px}
/* Weg */
.way{display:flex;gap:0;margin:22px 0 0;flex-wrap:wrap}
.way div{flex:1;min-width:130px;padding:9px 12px 9px 20px;color:#fff;font-weight:700;font-size:14px;position:relative;clip-path:polygon(0 0,calc(100% - 14px) 0,100% 50%,calc(100% - 14px) 100%,0 100%,14px 50%);margin-right:-6px}
.way div:first-child{clip-path:polygon(0 0,calc(100% - 14px) 0,100% 50%,calc(100% - 14px) 100%,0 100%);padding-left:14px}
.way small{display:block;font-weight:500;font-size:11px;opacity:.9}
.w1{background:var(--coral)}.w2{background:var(--amber);color:var(--navy)!important}.w3{background:var(--teal)}.w4{background:var(--violet)}.w5{background:var(--green)}
main{padding:26px 0 60px}
.intro{display:grid;grid-template-columns:1.2fr 1fr;gap:18px;margin-bottom:26px}
@media(max-width:760px){.intro{grid-template-columns:1fr}}
.panel{background:var(--card);border:1px solid var(--line);border-radius:14px;padding:16px 18px}
.panel h3{margin:0 0 6px;font-size:17px}
.panel ul{margin:6px 0 0 18px;padding:0}
.legend span{display:inline-block;margin-right:14px;font-size:14px}
.lv{display:inline-block;font-size:11px;font-weight:800;padding:2px 8px;border-radius:20px;letter-spacing:.04em;color:#fff;vertical-align:middle}
.l1{background:#2a9d8f}.l2{background:#e9a000;color:#14213D}.l3{background:#c0392b}
h2.ph{font-size:22px;margin:30px 0 4px;display:flex;align-items:center;gap:10px}
h2.ph i{display:inline-block;width:14px;height:26px;border-radius:4px;background:var(--c)}
.phsub{margin:0 0 12px;color:var(--mute);font-size:15px}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:14px}
.card{background:var(--card);border:2px solid var(--line);border-top:7px solid var(--c);border-radius:14px;padding:14px 16px 16px;text-align:left;transition:transform .15s,box-shadow .15s;position:relative;min-height:150px;display:flex;flex-direction:column}
.card:hover:not(.locked){transform:translateY(-3px);box-shadow:0 8px 20px rgba(20,33,61,.12)}
.card .no{font-size:12px;font-weight:800;color:var(--c);letter-spacing:.08em}
.card h4{margin:2px 0 4px;font-size:18px;line-height:1.2}
.card p{margin:0 0 8px;font-size:14px;color:var(--mute)}
.card .meta{margin-top:auto;display:flex;justify-content:space-between;align-items:center;font-size:13px;color:var(--mute)}
.card.done{border-color:var(--c);background:linear-gradient(180deg,#fff 0%,#f4fbf6 100%)}
.stamp{position:absolute;right:12px;top:14px;border:3px solid var(--green);color:var(--green);font-weight:900;font-size:12px;padding:1px 8px;border-radius:6px;transform:rotate(8deg);letter-spacing:.08em}
.card.locked{opacity:.55;background:#f5f2ea}
.lockline{font-size:12px;font-weight:700;color:#8a6d00}
.pill{background:#eef3f6;border-radius:20px;padding:2px 9px;font-size:12px;font-weight:700}
.pill.req{background:#fdebe5;color:#b33c1a}.pill.opt{background:#e8f4ea;color:#2f7a33}
/* Overlay */
#ov{position:fixed;inset:0;background:rgba(10,18,36,.72);display:none;z-index:50;overflow-y:auto;-webkit-overflow-scrolling:touch}
#ov.on{display:block}
.sheet{background:var(--paper);max-width:900px;margin:22px auto;border-radius:16px;overflow:hidden;box-shadow:0 20px 60px rgba(0,0,0,.4)}
.sh-head{background:var(--c);color:#fff;padding:16px 22px;display:flex;justify-content:space-between;gap:12px;align-items:flex-start}
.sh-head h2{margin:2px 0 0;font-size:26px;line-height:1.15}
.sh-head .no{font-size:12px;font-weight:800;letter-spacing:.12em;opacity:.9}
.x{background:rgba(255,255,255,.2);color:#fff;border:0;border-radius:8px;padding:8px 14px;font-weight:700}
.sh-body{padding:18px 22px 26px}
.info{background:#fff;border:1px solid var(--line);border-left:6px solid var(--c);border-radius:10px;padding:12px 16px;margin:12px 0}
.info b.k{color:var(--c)}
.mission{background:#FFF4D6;border:2px dashed var(--amber);border-radius:12px;padding:12px 16px;margin:12px 0}
.task{background:#fff;border:1px solid var(--line);border-radius:12px;padding:14px 16px;margin:14px 0;position:relative}
.task.ok{border-color:var(--c);background:#f7fcf8}
.th{display:flex;gap:10px;align-items:center;margin-bottom:6px;flex-wrap:wrap}
.tid{font-weight:800;color:var(--c)}
.field{margin-left:auto;font-size:12px;font-weight:800;background:var(--c);color:#fff;padding:2px 9px;border-radius:6px}
.op{background:#14213D;color:#fff;padding:0 7px;border-radius:5px;font-weight:800;margin-right:3px}
.star{background:#ede7ff;color:#5a3fa3;font-size:11px;font-weight:800;padding:2px 8px;border-radius:20px}
.tb{display:flex;gap:8px;flex-wrap:wrap;margin-top:10px;align-items:center}
.btn{background:var(--c);color:#fff;border:0;border-radius:9px;padding:8px 14px;font-weight:700}
.btn.sec{background:#eef3f6;color:var(--ink)}
.btn:disabled{opacity:.45;cursor:not-allowed}
.hint,.solu{margin-top:10px;border-radius:10px;padding:10px 14px;font-size:15px}
.hint{background:#FFF4D6;border:1px solid #f0d890}
.solu{background:#EAF3FF;border:1px solid #b9d3f3}
.chk{display:flex;align-items:center;gap:7px;font-size:14px;color:var(--mute);margin-left:auto}
.chk input{width:20px;height:20px;accent-color:var(--green)}
.fig{display:flex;gap:14px;flex-wrap:wrap;justify-content:center;margin:12px 0}
.fig figure{margin:0;background:#fff;border:1px solid var(--line);border-radius:12px;padding:8px 8px 6px;text-align:center;flex:1;min-width:220px;max-width:420px}
.fig figcaption{font-size:13px;font-weight:700;color:var(--navy)}
.fig svg{width:100%;height:auto;max-height:260px}
.note{font-size:12px;color:var(--mute);text-align:center;margin:-4px 0 8px}
.opts{display:flex;flex-direction:column;gap:8px;margin:8px 0}
.opt{border:2px solid var(--line);background:#fff;border-radius:10px;padding:10px 12px;text-align:left}
.opt.sel{border-color:var(--c);background:#f3f8ff}
.opt.right{border-color:#2f9e44;background:#ebfbee}.opt.wrong{border-color:#e03131;background:#fff0f0}
.row{display:flex;gap:8px;align-items:center;flex-wrap:wrap;padding:7px 0;border-bottom:1px dashed var(--line)}
.row span.t{flex:1;min-width:200px}
.sw{font-variant-numeric:tabular-nums;font-size:44px;font-weight:800;text-align:center;color:var(--navy)}
input.num,select,textarea{font:inherit;padding:7px 9px;border-radius:8px;border:2px solid var(--line);background:#fff;max-width:100%}
input.num{width:90px}
.ok-t{color:#2f7a33;font-weight:700}.bad-t{color:#c0392b;font-weight:700}
.fb{margin-top:8px;font-weight:600}
.chip{display:inline-block;background:#fff;border:2px solid var(--line);border-radius:20px;padding:5px 12px;margin:3px;font-size:14px}
.sticker{display:inline-block;background:var(--coral);color:#fff;border-radius:16px;padding:12px 18px;font-weight:800;font-size:20px;position:relative;margin:6px 0}
@media print{#ov{display:none!important}}
</style>
</head>
<body>
<header class="hero"><div class="wrap">
 <span class="tag">FALLAKTE BIOLOGIE 8</span>
 <h1>Stammt der Mensch vom Affen ab?</h1>
 <p class="lead">Du bist Teil eines Ermittlerteams. Sichere Spuren, führe Versuche durch und prüfe deine Hypothese an Beweisen, nicht an Meinungen.</p>
 <div class="way">
  <div class="w1">1 Problem<small>die Behauptung</small></div>
  <div class="w2">2 Hypothese<small>meine Vermutung</small></div>
  <div class="w3">3 Lösungsweg<small>Spuren, Versuche</small></div>
  <div class="w4">4 Erkenntnis<small>Auswertung</small></div>
  <div class="w5">5 Transfer<small>anwenden</small></div>
 </div>
 <div class="top">
  <input id="name" placeholder="Name des Teams" aria-label="Name des Teams">
  <div class="bar"><small id="ptxt">Fortschritt</small><div class="track"><div class="fill" id="fill"></div></div></div>
  <button class="ghost" id="reset">Neu starten</button>
 </div>
</div></header>
<main><div class="wrap">
 <section class="intro">
  <div class="panel"><h3>So arbeitest du</h3>
   <ul>
    <li>Arbeitet zu zweit mit einem Gerät. Jede Person füllt ihr eigenes Arbeitsblatt aus.</li>
    <li>Jede Aufgabe nennt das <b>Feld</b> auf dem Arbeitsblatt, in das du schreibst.</li>
    <li>Denke zuerst selbst und schreibe auf. Erst danach: <b>Tipp</b>, dann <b>Musterlösung</b>.</li>
    <li>Stationen mit Schloss öffnen sich, wenn die Schritte davor erledigt sind.</li>
   </ul></div>
  <div class="panel legend"><h3>Schwierigkeit</h3>
   <p style="margin:4px 0"><span><span class="lv l1">BASIS</span> beobachten, beschreiben</span></p>
   <p style="margin:4px 0"><span><span class="lv l2">AUFBAU</span> vergleichen, erklären</span></p>
   <p style="margin:4px 0"><span><span class="lv l3">TRANSFER</span> beurteilen, anwenden</span></p>
   <p style="margin:8px 0 0;font-size:14px"><span class="star">ZUSATZ</span> Aufgaben mit diesem Zeichen sind freiwillig, wenn die Zeit knapp wird.</p>
   <p style="margin:8px 0 0;font-size:14px;color:var(--mute)">Zeitrahmen: zwei Schulstunden (90 Minuten).</p></div>
 </section>
 <div id="home"></div>
</div></main>
<div id="ov" role="dialog" aria-modal="true"><div class="sheet" id="sheet"></div></div>
<script>
/* ===== Eigene Schemazeichnungen (stark vereinfacht, nicht maßstäblich) ===== */
const PINK='#e87aa8',BLUE='#5aa5e0',BONE='#d9c9a8',DK='#14213D';
const W=(vb,inner)=>`<svg viewBox="${vb}" xmlns="http://www.w3.org/2000/svg" role="img">${inner}</svg>`;
const rad=d=>d*Math.PI/180;
function skull(k){
  const cubes=n=>Array.from({length:n},(_,i)=>`<rect x="${12+i*17}" y="146" width="14" height="14" fill="${PINK}" stroke="${DK}" stroke-width="1"/>`).join('');
  if(k==='m') return W('0 0 200 168',`
   <ellipse cx="85" cy="62" rx="58" ry="50" fill="${PINK}" stroke="${DK}" stroke-width="2"/>
   <path d="M112 78 L148 88 L150 112 L124 132 L98 122 L94 96Z" fill="${BLUE}" stroke="${DK}" stroke-width="2"/>
   <circle cx="116" cy="82" r="7" fill="#fff" stroke="${DK}"/><path d="M106 70 Q116 66 126 72" fill="none" stroke="${DK}" stroke-width="2"/>
   <text x="12" y="142" font-size="10" fill="${DK}" font-family="Arial">Gehirnvolumen:</text>${cubes(3)}`);
  return W('0 0 200 168',`
   <ellipse cx="68" cy="72" rx="38" ry="30" fill="${PINK}" stroke="${DK}" stroke-width="2"/>
   <path d="M92 66 L170 80 L174 118 L140 128 L96 114Z" fill="${BLUE}" stroke="${DK}" stroke-width="2"/>
   <circle cx="108" cy="82" r="7" fill="#fff" stroke="${DK}"/><path d="M92 70 Q108 60 124 72" fill="none" stroke="${DK}" stroke-width="7" stroke-linecap="round"/>
   <text x="12" y="142" font-size="10" fill="${DK}" font-family="Arial">Gehirnvolumen:</text>${cubes(1)}`);
}
function teeth(k){
  let s='';
  if(k==='m'){
    for(let i=0;i<16;i++){const t=-1.45+i*(2.9/15);const x=100+62*Math.sin(t),y=34+88*(1-Math.cos(t));
      const c=(i===5||i===10);s+=`<circle cx="${x.toFixed(1)}" cy="${y.toFixed(1)}" r="${c?6.5:7}" fill="${c?'#f4b4a2':'#fff'}" stroke="${DK}" stroke-width="1.6"/>`;}
    return W('0 0 200 150',`<path d="M38 124 C38 10 162 10 162 124" fill="none" stroke="#e9d6c0" stroke-width="22" stroke-linecap="round"/>${s}`);
  }
  [85,95,105,115].forEach(x=>{s+=`<circle cx="${x}" cy="30" r="5.5" fill="#fff" stroke="${DK}" stroke-width="1.6"/>`;});
  s+=`<path d="M60 30 L72 30 L66 66Z M128 30 L140 30 L134 66Z" fill="#f4b4a2" stroke="${DK}" stroke-width="1.6"/>`;
  [50,150].forEach(x=>{for(let i=0;i<5;i++){const y=84+i*11;s+=`<circle cx="${x}" cy="${y}" r="${i<2?5.5:7}" fill="#fff" stroke="${DK}" stroke-width="1.6"/>`;}});
  return W('0 0 200 150',`<path d="M50 138 L50 30 L150 30 L150 138" fill="none" stroke="#e9d6c0" stroke-width="22" stroke-linejoin="round"/>${s}`);
}
function spine(k){
  let pts=[];for(let i=0;i<24;i++){const y=i/23;const x=k==='m'?60+15*Math.sin(3*Math.PI*y+0.3):30+44*Math.sin(Math.PI*y*0.92);pts.push([x,22+y*188]);}
  const d='M'+pts.map(p=>p.map(v=>v.toFixed(1)).join(' ')).join(' L');
  const v=pts.map((p,i)=>`<circle cx="${p[0].toFixed(1)}" cy="${p[1].toFixed(1)}" r="${(4+i*0.12).toFixed(1)}" fill="${BONE}" stroke="${DK}" stroke-width="1.2"/>`).join('');
  return W('0 0 130 230',`<ellipse cx="${pts[0][0]-2}" cy="12" rx="13" ry="10" fill="${PINK}" stroke="${DK}" stroke-width="1.5"/><path d="${d}" fill="none" stroke="#bfae8a" stroke-width="3"/>${v}<line x1="8" y1="218" x2="122" y2="218" stroke="#9aa5b1" stroke-width="1.5"/><text x="65" y="228" text-anchor="middle" font-size="9" fill="#6b7782" font-family="Arial">Boden</text>`);
}
function ribs(k){
  const hw=y=>k==='m'?36+24*Math.sin(Math.PI*(0.05+0.9*y)):14+46*y;
  let L=[],R=[];for(let i=0;i<=20;i++){const y=i/20;L.push([80-hw(y),12+y*160]);R.push([80+hw(y),12+y*160]);}
  const outline='M'+L.map(p=>p.join(' ')).join(' L')+' L'+R.reverse().map(p=>p.join(' ')).join(' L')+'Z';
  let r='';for(let y=0.1;y<=0.95;y+=0.12){const yy=12+y*160,h=hw(y);r+=`<path d="M${80-h} ${yy} Q80 ${yy+16} ${80+h} ${yy}" fill="none" stroke="${DK}" stroke-width="2"/>`;}
  return W('0 0 160 190',`<path d="${outline}" fill="#f6efe0" stroke="${DK}" stroke-width="2.2"/>${r}<line x1="80" y1="12" x2="80" y2="172" stroke="#bfae8a" stroke-width="5"/>`);
}
function pelvis(k){
  const d=k==='m'?'M15 25 C5 60 30 95 80 100 C130 95 155 60 145 25 C125 40 105 38 80 40 C55 38 35 40 15 25Z':'M48 6 C36 60 52 116 80 140 C108 116 124 60 112 6 C102 22 94 26 80 26 C66 26 58 22 48 6Z';
  const h=k==='m'?'<ellipse cx="80" cy="62" rx="22" ry="17" fill="#fff" stroke="#14213D" stroke-width="2"/>':'<ellipse cx="80" cy="76" rx="11" ry="26" fill="#fff" stroke="#14213D" stroke-width="2"/>';
  return W('0 0 160 150',`<path d="${d}" fill="${BONE}" stroke="${DK}" stroke-width="2.2"/>${h}`);
}
function limb(parts){return parts.map(([x,y,a,l,w])=>{const x2=x+l*Math.sin(rad(a)),y2=y-l*Math.cos(rad(a));return `<line x1="${x}" y1="${y}" x2="${x2.toFixed(1)}" y2="${y2.toFixed(1)}" stroke="${BONE}" stroke-width="${w}" stroke-linecap="round"/><line x1="${x}" y1="${y}" x2="${x2.toFixed(1)}" y2="${y2.toFixed(1)}" stroke="${DK}" stroke-width="1" stroke-linecap="round" opacity=".5"/>`}).join('');}
function hand(k){
  const f=k==='m'?[[48,92,-18,46,10],[58,88,-6,54,10],[68,88,6,50,10],[78,92,18,40,9],[40,112,-62,40,12]]:[[48,92,-18,56,9],[58,88,-6,66,9],[68,88,6,62,9],[78,92,18,50,8],[40,112,-66,34,11]];
  return W('0 0 120 150',limb(f)+`<ellipse cx="62" cy="108" rx="26" ry="26" fill="${BONE}" stroke="${DK}" stroke-width="2"/>`);
}
function foot(k){
  const f=k==='m'?[[50,78,-4,36,15],[60,74,2,28,10],[68,74,6,26,9],[76,78,10,22,8],[82,84,14,18,7]]:[[56,84,6,44,9],[66,82,10,46,9],[76,84,14,42,8],[84,90,18,36,7],[42,104,-66,38,12]];
  const e=k==='m'?'<ellipse cx="64" cy="112" rx="24" ry="34" fill="'+BONE+'" stroke="'+DK+'" stroke-width="2"/>':'<ellipse cx="66" cy="116" rx="19" ry="30" fill="'+BONE+'" stroke="'+DK+'" stroke-width="2"/>';
  return W('0 0 120 160',limb(f)+e);
}
function figure(k){
  const m=k==='m';
  const sh=m?[110,46]:[110,62], hip=m?[110,112]:[110,126], arm=m?70:85, leg=m?100:55;
  return W('0 0 220 256',`
   <circle cx="110" cy="${sh[1]-24}" r="14" fill="${PINK}" stroke="${DK}" stroke-width="1.5"/>
   <line x1="110" y1="${sh[1]-10}" x2="${hip[0]}" y2="${hip[1]}" stroke="${DK}" stroke-width="5" stroke-linecap="round"/>
   <line x1="88" y1="${sh[1]}" x2="132" y2="${sh[1]}" stroke="${DK}" stroke-width="5" stroke-linecap="round"/>
   <line x1="88" y1="${sh[1]}" x2="82" y2="${sh[1]+arm}" stroke="${BLUE}" stroke-width="6" stroke-linecap="round"/>
   <line x1="132" y1="${sh[1]}" x2="138" y2="${sh[1]+arm}" stroke="${BLUE}" stroke-width="6" stroke-linecap="round"/>
   <line x1="100" y1="${hip[1]}" x2="96" y2="${hip[1]+leg}" stroke="${PINK}" stroke-width="7" stroke-linecap="round"/>
   <line x1="120" y1="${hip[1]}" x2="124" y2="${hip[1]+leg}" stroke="${PINK}" stroke-width="7" stroke-linecap="round"/>
   <text x="12" y="232" font-size="12" font-weight="700" fill="#2c6aa0" font-family="Arial">Arm: ${arm} Einheiten</text>
   <text x="12" y="247" font-size="12" font-weight="700" fill="#c4568a" font-family="Arial">Bein: ${leg} Einheiten</text>`);
}
function tree(){return W('0 0 240 150',`<path d="M120 130 C120 100 60 100 60 40" fill="none" stroke="${DK}" stroke-width="3"/><path d="M120 130 C120 100 180 100 180 40" fill="none" stroke="${DK}" stroke-width="3"/>
 <rect x="20" y="14" width="80" height="26" rx="6" fill="#fff" stroke="${DK}" stroke-width="2"/><rect x="140" y="14" width="80" height="26" rx="6" fill="#fff" stroke="${DK}" stroke-width="2"/><rect x="70" y="124" width="100" height="24" rx="6" fill="#fff" stroke="${DK}" stroke-width="2"/>
 <text x="60" y="31" text-anchor="middle" font-size="13" font-family="Arial">A</text><text x="180" y="31" text-anchor="middle" font-size="13" font-family="Arial">B</text><text x="120" y="140" text-anchor="middle" font-size="13" font-family="Arial">C</text>`);}
const fig2=(a,ca,b,cb,note)=>`<div class="fig"><figure>${a}<figcaption>${ca}</figcaption></figure><figure>${b}<figcaption>${cb}</figcaption></figure></div>${note===false?'':'<div class="note">Schemazeichnung, stark vereinfacht und nicht maßstäblich</div>'}`;
/* ===== Zustand ===== */
const KEY='fallakte_mensch_affe_v1';
let S={name:'',hyp:null,done:{},st:{},polls:{},};
try{const r=localStorage.getItem(KEY);if(r)S=Object.assign(S,JSON.parse(r));}catch(e){}
const save=()=>{try{localStorage.setItem(KEY,JSON.stringify(S));}catch(e){}};
const $=s=>document.querySelector(s);
const HYP={H1:'Der Mensch hat sich aus dem heutigen Schimpansen entwickelt.',H2:'Mensch und heutiger Schimpanse haben gemeinsame Vorfahren, aber keiner stammt vom anderen ab.',H3:'Mensch und Schimpanse sind nicht miteinander verwandt.'};
const LV={1:['BASIS','l1'],2:['AUFBAU','l2'],3:['TRANSFER','l3']};
let pending=[];
/* ===== Widgets ===== */
const WG={};
WG.hypo=(el)=>{
  const draw=()=>{
    const lock=!!S.hyp;
    el.innerHTML=`<div class="opts">${Object.entries(HYP).map(([k,t])=>`<button class="opt ${S.hyp===k?'sel':''}" data-k="${k}" ${lock?'disabled':''}><b>${k}</b> ${t}</button>`).join('')}</div>
    <div class="tb">${lock?'<span class="ok-t">Hypothese festgehalten. Sie bleibt sichtbar, bis du sie in der Auswertung prüfst.</span>':'<button class="btn" id="hcommit" disabled>Hypothese festhalten</button>'}</div>`;
    if(!lock){let sel=null;el.querySelectorAll('.opt').forEach(b=>b.onclick=()=>{sel=b.dataset.k;el.querySelectorAll('.opt').forEach(x=>x.classList.toggle('sel',x===b));el.querySelector('#hcommit').disabled=false;});
      el.querySelector('#hcommit').onclick=()=>{S.hyp=sel;save();draw();refreshGates();};}
  };draw();
};
WG.poll=(el,c)=>{
  const draw=()=>{const v=S.polls[c.key];
    el.innerHTML=`<div class="opts">${c.opts.map((o,i)=>`<button class="opt ${v===i?'sel':''}" data-i="${i}">${o}</button>`).join('')}</div>${v!=null?'<div class="fb ok-t">Vermutung festgehalten. Trage sie ins Arbeitsblatt ein, dann teste sie.</div>':''}`;
    el.querySelectorAll('.opt').forEach(b=>b.onclick=()=>{S.polls[c.key]=+b.dataset.i;save();draw();});};draw();
};
WG.assign=(el,c)=>{
  const ans=S.polls['as_'+c.key]||{};
  el.innerHTML=c.items.map((it,i)=>`<div class="row" data-i="${i}"><span class="t">${it[0]}</span>${c.opts.map((o,j)=>`<button class="btn sec" data-j="${j}">${o}</button>`).join('')}<span class="mk"></span></div>`).join('')+`<div class="tb"><button class="btn" id="chk">Prüfen</button><span class="fb" id="fb"></span></div>`;
  const sel={};
  el.querySelectorAll('.row').forEach(r=>{const i=+r.dataset.i;r.querySelectorAll('button').forEach(b=>b.onclick=()=>{sel[i]=+b.dataset.j;r.querySelectorAll('button').forEach(x=>{x.classList.toggle('sec',x!==b);});r.querySelector('.mk').textContent='';});});
  el.querySelector('#chk').onclick=()=>{let ok=0;el.querySelectorAll('.row').forEach(r=>{const i=+r.dataset.i;const m=r.querySelector('.mk');if(sel[i]===undefined){m.textContent='';return;}
    const good=sel[i]===c.items[i][1];if(good)ok++;m.innerHTML=good?'<span class="ok-t">richtig</span>':'<span class="bad-t">noch einmal überlegen</span>';});
    el.querySelector('#fb').textContent=ok===c.items.length?'Alles richtig.':ok+' von '+c.items.length+' richtig. Korrigiere die markierten Zeilen.';};
};
WG.modelmap=(el,c)=>{
  el.innerHTML=`<table style="width:100%;border-collapse:collapse">${c.rows.map((r,i)=>`<tr><td style="padding:6px 8px;border-bottom:1px dashed #e3dccb"><b>${r[0]}</b> im Modell steht für</td><td style="padding:6px 0;border-bottom:1px dashed #e3dccb"><select data-i="${i}"><option value="">wähle</option>${c.opts.map((o,j)=>`<option value="${j}">${o}</option>`).join('')}</select> <span class="mk"></span></td></tr>`).join('')}</table><div class="tb"><button class="btn" id="chk">Prüfen</button></div>`;
  el.querySelector('#chk').onclick=()=>el.querySelectorAll('select').forEach(s=>{const i=+s.dataset.i;const m=s.parentNode.querySelector('.mk');if(s.value==='')return;m.innerHTML=(+s.value===c.rows[i][1])?'<span class="ok-t">richtig</span>':'<span class="bad-t">nein, überlege noch einmal</span>';});
};
WG.stopwatch=(el)=>{
  let t0=0,run=false,acc=0,iv,laps=[];
  el.innerHTML=`<div class="sw" id="d">0,00 s</div><div class="tb" style="justify-content:center"><button class="btn" id="go">Start</button><button class="btn sec" id="lap">Zeit merken</button><button class="btn sec" id="rs">Zurücksetzen</button></div><div id="laps" style="text-align:center;margin-top:8px;color:var(--mute)"></div>`;
  const d=el.querySelector('#d'),go=el.querySelector('#go');
  const cur=()=>acc+(run?(performance.now()-t0)/1000:0);
  const show=()=>d.textContent=cur().toFixed(2).replace('.',',')+' s';
  go.onclick=()=>{if(run){acc=cur();run=false;clearInterval(iv);go.textContent='Weiter';}else{t0=performance.now();run=true;iv=setInterval(show,50);go.textContent='Stopp';}show();};
  el.querySelector('#lap').onclick=()=>{laps.push(cur().toFixed(2).replace('.',','));el.querySelector('#laps').innerHTML=laps.map((l,i)=>`<span class="chip">${i+1}: ${l} s</span>`).join('');};
  el.querySelector('#rs').onclick=()=>{run=false;clearInterval(iv);acc=0;go.textContent='Start';show();};
};
WG.ratio=(el,c)=>{
  el.innerHTML=`<div class="row"><span class="t">Verhältnis Arm : Bein beim <b>Menschen</b> (Arm geteilt durch Bein)</span><input class="num" id="a" inputmode="decimal"></div><div class="row"><span class="t">Verhältnis Arm : Bein beim <b>Schimpansen</b></span><input class="num" id="b" inputmode="decimal"></div><div class="tb"><button class="btn" id="chk">Prüfen</button><span class="fb" id="fb"></span></div>`;
  el.querySelector('#chk').onclick=()=>{const g=id=>parseFloat(el.querySelector(id).value.replace(',','.'));const a=g('#a'),b=g('#b');
    const oa=Math.abs(a-c.a)<0.06,ob=Math.abs(b-c.b)<0.06;
    el.querySelector('#fb').innerHTML=(isNaN(a)||isNaN(b))?'Fülle beide Felder aus.':(oa&&ob?'<span class="ok-t">Beide Werte stimmen (auf zwei Stellen gerundet).</span>':'<span class="bad-t">'+(oa?'':'Menschenwert ')+(ob?'':'Schimpansenwert ')+'stimmt noch nicht. Rechne Armlänge geteilt durch Beinlänge.</span>');};
};
WG.bite=(el)=>{
  let mode='gap',v=0;
  const draw=()=>{
    const maxV=100,lim=mode==='gap'?100:44,vv=Math.min(v,lim),lowY=150-vv*0.62,blocked=mode==='nogap'&&v>lim;
    const lower=mode==='gap'
      ?`<rect x="30" y="${lowY}" width="240" height="40" rx="6" fill="#e9d6c0" stroke="${DK}" stroke-width="2"/>${[40,60,80,100,200,220,240].map(x=>`<rect x="${x}" y="${lowY-10}" width="14" height="12" rx="3" fill="#fff" stroke="${DK}"/>`).join('')}`
      :`<rect x="30" y="${lowY}" width="240" height="40" rx="6" fill="#e9d6c0" stroke="${DK}" stroke-width="2"/>${[40,60,80,100,120,140,160,180,200,220,240].map(x=>`<rect x="${x}" y="${lowY-10}" width="14" height="12" rx="3" fill="#fff" stroke="${DK}"/>`).join('')}`;
    el.innerHTML=`<div class="fig"><figure style="max-width:560px">${W('0 0 300 210',`<rect x="30" y="20" width="240" height="40" rx="6" fill="#e9d6c0" stroke="${DK}" stroke-width="2"/>${[40,60,80,100,200,220,240].map(x=>`<rect x="${x}" y="58" width="14" height="12" rx="3" fill="#fff" stroke="${DK}"/>`).join('')}<path d="M118 58 L132 58 L125 112Z" fill="#f4b4a2" stroke="${DK}" stroke-width="1.6"/><path d="M168 58 L182 58 L175 112Z" fill="#f4b4a2" stroke="${DK}" stroke-width="1.6"/>${lower}`)}<figcaption>Oberkiefer (oben) und Unterkiefer (unten), Seitenansicht des Schemas</figcaption></figure></div>
    <div class="row"><span class="t">Modell wählen:</span><button class="btn ${mode==='gap'?'':'sec'}" data-m="gap">Unterkiefer mit Lücke</button><button class="btn ${mode==='nogap'?'':'sec'}" data-m="nogap">Unterkiefer ohne Lücke</button></div>
    <div class="row"><span class="t">Kiefer schließen:</span><input type="range" min="0" max="100" value="${v}" id="sl" style="flex:1;min-width:160px"></div>
    <div class="fb">${blocked?'<span class="bad-t">Die langen Zähne stoßen auf den Unterkiefer. Der Mund lässt sich nicht ganz schließen.</span>':(v>=98?'<span class="ok-t">Der Mund ist ganz geschlossen.</span>':'')}</div>`;
    el.querySelectorAll('[data-m]').forEach(b=>b.onclick=()=>{mode=b.dataset.m;draw();});
    const sl=el.querySelector('#sl');sl.oninput=()=>{v=+sl.value;draw();el.querySelector('#sl').focus();};
  };draw();
};
WG.balance=(el)=>{
  let m='m';
  const draw=()=>{
    const body=m==='m'?`<path d="M118 205 C124 170 104 140 116 112 C126 88 114 66 118 48" fill="none" stroke="${DK}" stroke-width="6" stroke-linecap="round"/><circle cx="118" cy="34" r="14" fill="${PINK}" stroke="${DK}" stroke-width="2"/>`:`<path d="M112 205 C108 170 110 150 104 128 C116 102 142 84 160 64" fill="none" stroke="${DK}" stroke-width="6" stroke-linecap="round"/><circle cx="172" cy="56" r="14" fill="${PINK}" stroke="${DK}" stroke-width="2"/>`;
    const cx=m==='m'?117:136,cy=m==='m'?124:112;
    const inside=cx>=96&&cx<=136;
    el.innerHTML=`<div class="fig"><figure style="max-width:520px">${W('0 0 260 240',`<line x1="10" y1="212" x2="250" y2="212" stroke="${DK}" stroke-width="3"/><rect x="96" y="208" width="40" height="8" fill="${BLUE}"/><text x="116" y="232" text-anchor="middle" font-size="10" font-family="Arial" fill="#2c6aa0">Standfläche der Füße</text>${body}<circle cx="${cx}" cy="${cy}" r="7" fill="${C_AMBER}" stroke="${DK}" stroke-width="2"/><line x1="${cx}" y1="${cy+7}" x2="${cx}" y2="212" stroke="#c0392b" stroke-width="2" stroke-dasharray="4 3"/><text x="${cx+10}" y="${cy-8}" font-size="10" font-family="Arial" fill="${DK}">Körperschwerpunkt</text>`)}<figcaption>${m==='m'?'Mensch steht aufrecht':'Schimpanse steht aufrecht auf zwei Beinen'}</figcaption></figure></div>
    <div class="row"><button class="btn ${m==='m'?'':'sec'}" data-m="m">Mensch</button><button class="btn ${m==='s'?'':'sec'}" data-m="s">Schimpanse</button><span class="fb">${inside?'<span class="ok-t">Das rote Lot trifft die Standfläche: stabil.</span>':'<span class="bad-t">Das rote Lot trifft vor die Standfläche: Der Körper kippt nach vorne.</span>'}</span></div>`;
    el.querySelectorAll('[data-m]').forEach(b=>b.onclick=()=>{m=b.dataset.m;draw();});
  };draw();
};
const C_AMBER='#F2A900';
WG.treeassign=(el)=>{
  const o=`<option value="">wähle</option><option>Mensch</option><option>Schimpanse</option><option>gemeinsame Vorfahren</option>`;
  el.innerHTML=`<div class="fig"><figure style="max-width:420px">${tree()}<figcaption>Oben: heute. Unten: früher</figcaption></figure></div>
  <div class="row"><span class="t">Feld A <select data-p="A">${o}</select> &nbsp; Feld B <select data-p="B">${o}</select> &nbsp; Feld C <select data-p="C">${o}</select></span></div><div class="tb"><button class="btn" id="chk">Prüfen</button><span class="fb" id="fb"></span></div>`;
  el.querySelector('#chk').onclick=()=>{const g=p=>el.querySelector(`[data-p=${p}]`).value;const a=g('A'),b=g('B'),c=g('C');
    const ok=c==='gemeinsame Vorfahren'&&((a==='Mensch'&&b==='Schimpanse')||(a==='Schimpanse'&&b==='Mensch'));
    el.querySelector('#fb').innerHTML=ok?'<span class="ok-t">Richtig: Beide Äste beginnen bei denselben Vorfahren.</span>':'<span class="bad-t">Noch nicht. Überlege, wer unten an der Wurzel steht und wer oben an den Ästen.</span>';};
};
/* ===== Rendering ===== */
const esc=s=>s;
function taskHTML(t,st){
  const L=LV[t.lvl];
  const w=t.w?`<div class="wg" id="wg-${t.id}"></div>`:'';
  if(t.w)pending.push([`wg-${t.id}`,t.w.n,t.w.c]);
  return `<div class="task ${S.done[t.id]?'ok':''}" id="t-${t.id}" style="--c:${st.c}">
   <div class="th"><span class="tid">${t.id}</span><span class="lv ${L[1]}">${L[0]}</span>${t.star?'<span class="star">ZUSATZ</span>':''}<span class="field">${t.field}</span></div>
   <div><span class="op">${t.op}</span> ${t.text}</div>${w}
   <div class="tb"><button class="btn sec" data-a="hint" data-id="${t.id}">Tipp</button><button class="btn sec" data-a="sol" data-id="${t.id}">Musterlösung</button>
   <label class="chk"><input type="checkbox" data-a="done" data-id="${t.id}" ${S.done[t.id]?'checked':''}> erledigt und eingetragen</label></div>
   <div id="h-${t.id}"></div><div id="s-${t.id}"></div></div>`;
}
const TASKS={};
function sheetHTML(st){
  pending=[];
  const body=st.blocks.map(b=>{
    if(b.t==='html')return b.h;
    if(b.t==='fn')return b.f();
    if(b.t==='w'){const id='wb'+Math.random().toString(36).slice(2,8);pending.push([id,b.n,b.c]);return `<div class="wg" id="${id}"></div>`;}
    if(b.t==='task'){TASKS[b.id]=b;return taskHTML(b,st);}
    return '';}).join('');
  return `<div class="sh-head" style="--c:${st.c};background:${st.c}"><div><div class="no">${st.no}</div><h2>${st.title}</h2></div><button class="x" id="xx">Schließen</button></div>
  <div class="sh-body" style="--c:${st.c}">${body}<div class="tb" style="margin-top:22px;justify-content:space-between"><span id="sgate" class="fb"></span><button class="btn" id="secure" style="background:${st.c}">${st.fin}</button></div></div>`;
}
let cur=null;
function openSt(id){
  const st=STATIONS.find(s=>s.id===id);cur=st;
  const sh=$('#sheet');sh.innerHTML=sheetHTML(st);
  pending.forEach(([i,n,c])=>{const el=document.getElementById(i);if(el)WG[n](el,c||{});});
  $('#ov').classList.add('on');$('#ov').scrollTop=0;document.body.style.overflow='hidden';
  $('#xx').onclick=closeSt;
  sh.onclick=e=>{const b=e.target.closest('[data-a]');if(!b)return;const id=b.dataset.id,t=TASKS[id];
    if(b.dataset.a==='hint'){const box=document.getElementById('h-'+id);const n=+(box.dataset.n||0);if(n<t.hints.length){box.dataset.n=n+1;box.innerHTML=t.hints.slice(0,n+1).map((h,i)=>`<div class="hint"><b>Tipp ${i+1}:</b> ${h}</div>`).join('');b.textContent=n+1<t.hints.length?'Nächster Tipp':'Alle Tipps gezeigt';}}
    if(b.dataset.a==='sol'){const box=document.getElementById('s-'+id);if(box.innerHTML){box.innerHTML='';b.textContent='Musterlösung';}else{if(!confirm('Hast du deine Antwort schon aufgeschrieben?'))return;box.innerHTML=`<div class="solu"><b>Musterlösung:</b> ${t.sol}</div>`;b.textContent='Musterlösung ausblenden';}}
    if(b.dataset.a==='done'){S.done[id]=b.checked;save();document.getElementById('t-'+id).classList.toggle('ok',b.checked);gate();}};
  $('#secure').onclick=()=>{S.st[st.id]=true;save();closeSt();};
  gate();
}
function need(st){return st.blocks.filter(b=>b.t==='task'&&!b.star).map(b=>b.id);}
function gate(){
  if(!cur)return;const miss=need(cur).filter(i=>!S.done[i]);
  const hy=cur.id==='s0'&&!S.hyp;
  const ok=miss.length===0&&!hy;
  $('#secure').disabled=!ok;
  $('#sgate').textContent=ok?'':(hy?'Halte zuerst deine Hypothese fest.':'Noch offen: '+miss.join(', ')+' (freiwillige Zusatzaufgaben zählen nicht).');
}
function closeSt(){$('#ov').classList.remove('on');document.body.style.overflow='';cur=null;renderHome();}
document.addEventListener('keydown',e=>{if(e.key==='Escape'&&cur)closeSt();});
/* ===== Startseite ===== */
function locked(st){
  const first=STATIONS.filter(s=>/^s[1-5]$/.test(s.id));
  if(st.id==='s0')return null;
  if(/^s[1-5]$/.test(st.id))return S.hyp?null:'Zuerst Station 0: Hypothese festhalten';
  if(st.id==='s6')return first.every(s=>S.st[s.id])?null:'Zuerst alle fünf Spuren sichern';
  return S.st.s6?null:'Zuerst die Auswertung abschließen';
}
function progress(){
  const req=['s0','s1','s2','s3','s4','s5','s6'];let n=req.filter(i=>S.st[i]).length;if(['t1','t2','t3'].some(i=>S.st[i]))n++;
  const p=Math.round(n/8*100);$('#fill').style.width=p+'%';$('#ptxt').textContent='Fortschritt: '+p+' Prozent'+(p===100?' | Fall gelöst, gute Arbeit.':'');
}
function renderHome(){
  const groups=[
   ['Problem und Hypothese','var(--coral)','Lege dich fest, bevor du Beweise siehst.',['s0']],
   ['Lösungsweg: Spuren sichern','var(--teal)','Fünf Spuren, fünf Skelettmerkmale. Reihenfolge frei.',['s1','s2','s3','s4','s5']],
   ['Erkenntnis: Auswertung','var(--violet)','Führe alle Ergebnisse zusammen und prüfe deine Hypothese.',['s6']],
   ['Transfer: Wende dein Wissen an','var(--green)','Wähle mindestens eine Aufgabe. Schnelle Teams schaffen alle drei.',['t1','t2','t3']]];
  $('#home').innerHTML=groups.map(([t,c,sub,ids])=>`<h2 class="ph" style="--c:${c}"><i></i>${t}</h2><p class="phsub">${sub}</p><div class="grid">${ids.map(id=>{const st=STATIONS.find(s=>s.id===id);const lk=locked(st);const dn=S.st[id];
    return `<button class="card ${lk?'locked':''} ${dn?'done':''}" style="--c:${st.c}" data-id="${id}"><span class="no">${st.no}</span>${dn?'<span class="stamp">GESICHERT</span>':''}<h4>${st.title}</h4><p>${st.teaser}</p>${lk?`<div class="lockline">Gesperrt: ${lk}</div>`:''}<div class="meta"><span class="pill ${st.opt?'opt':'req'}">${st.opt?'Wahl':'Pflicht'}</span><span>ca. ${st.min} Min.</span></div></button>`}).join('')}</div>`).join('');
  $('#home').querySelectorAll('.card').forEach(b=>b.onclick=()=>{const st=STATIONS.find(s=>s.id===b.dataset.id);const lk=locked(st);if(lk&&!confirm('Gesperrt. '+lk+'.\nTrotzdem öffnen? Frage zuerst deine Lehrkraft.'))return;openSt(st.id);});
  progress();
}
function refreshGates(){}
$('#name').value=S.name||'';$('#name').oninput=e=>{S.name=e.target.value;save();};
$('#reset').onclick=()=>{if(confirm('Wirklich alles zurücksetzen? Hypothese und Fortschritt gehen verloren.')){S={name:S.name,hyp:null,done:{},st:{},polls:{}};save();renderHome();}};
/* ===== Stationen 0 bis 3 ===== */
const STATIONS=[];
const mis=h=>({t:'html',h:`<div class="mission"><b>Dein Auftrag:</b> ${h}</div>`});
const H=h=>({t:'html',h});
function headspine(k){
  if(k==='m')return W('0 0 200 170',`<ellipse cx="90" cy="62" rx="56" ry="46" fill="${PINK}" stroke="${DK}" stroke-width="2"/><path d="M112 82 L148 90 L150 112 L124 130 L100 120 L96 98Z" fill="${BLUE}" stroke="${DK}" stroke-width="2"/><circle cx="118" cy="82" r="6" fill="#fff" stroke="${DK}"/><line x1="86" y1="106" x2="86" y2="168" stroke="#bfae8a" stroke-width="9"/><circle cx="86" cy="106" r="6" fill="#e03131" stroke="#fff" stroke-width="1.5"/>`);
  return W('0 0 200 170',`<ellipse cx="84" cy="62" rx="36" ry="28" fill="${PINK}" stroke="${DK}" stroke-width="2"/><path d="M106 58 L176 74 L180 112 L146 122 L108 108Z" fill="${BLUE}" stroke="${DK}" stroke-width="2"/><circle cx="118" cy="76" r="6" fill="#fff" stroke="${DK}"/><path d="M104 64 Q118 56 132 66" fill="none" stroke="${DK}" stroke-width="6" stroke-linecap="round"/><line x1="56" y1="82" x2="50" y2="168" stroke="#bfae8a" stroke-width="9"/><circle cx="56" cy="82" r="6" fill="#e03131" stroke="#fff" stroke-width="1.5"/>`);
}
STATIONS.push({id:'s0',no:'STATION 0',title:'Die Behauptung',teaser:'Lege deine Hypothese fest und plane, wie du sie prüfen willst.',c:'#E4572E',min:10,fin:'Station 0 abschließen',blocks:[
 H(`<div class="info"><div class="sticker">„Der Mensch stammt vom Affen ab!“</div><p>Diesen Satz hört man oft. Stimmt er? Und was würde er eigentlich bedeuten? Forschende legen sich zuerst auf eine <b class="k">Hypothese</b> fest und prüfen sie dann an Beweisen. Genau das machst du jetzt.</p></div>`),
 mis('Entscheide dich, bevor du Beweise siehst. Es gibt keine peinliche Antwort, aber am Ende wird geprüft.'),
 {t:'task',id:'0.1',lvl:2,op:'Formuliere',text:'Wähle eine der drei Hypothesen und begründe deine Entscheidung in ein bis zwei Sätzen auf dem Arbeitsblatt. Halte die Hypothese danach hier fest.',field:'Feld 1',w:{n:'hypo'},
  hints:['Was hast du schon über Menschen und Schimpansen gesehen oder gehört? Wo wirken sie ähnlich, wo verschieden?','Prüfe jede Hypothese mit einer Frage: Bei H1, warum gäbe es dann heute noch Schimpansen? Bei H3, wie erklärst du Ähnlichkeiten?'],
  sol:'Es gibt keine falsche Anfangshypothese. Wichtig ist eine Begründung, die sich überprüfen lässt. Am Ende der Stunde vergleichst du, ob die Beweise deine Hypothese stützen.'},
 {t:'task',id:'0.2',lvl:2,op:'Plane',text:'einen Lösungsweg: Nenne vier Körperbereiche, die du bei Mensch und Schimpanse vergleichen würdest. Lege außerdem ein Kriterium fest: Woran erkennst du, dass Ergebnisse für Verwandtschaft sprechen?',field:'Feld 2',
  hints:['Ein Skelett lässt sich von oben nach unten durchgehen.','Was muss bei zwei Verwandten gleich sein? Was darf sich unterscheiden, und aus welchem Grund?'],
  sol:'Mögliche Bereiche: Schädel, Gebiss, Wirbelsäule, Brustkorb, Becken, Arme und Beine, Hand, Fuß. Kriterium: Viele gleiche Bauteile; Unterschiede, die sich als Anpassung an eine andere Lebensweise erklären lassen.'},
 H(`<div class="info">Die fünf Spuren folgen genau diesen Bereichen. Du gehst jetzt wie Ermittler vor: Beobachten, Messen, Modell testen, Schlüsse ziehen.</div>`)]});

STATIONS.push({id:'s1',no:'SPUR 1',title:'Kopf und Gebiss',teaser:'Schädelproportionen, Zahnbögen und ein Biss-Modell.',c:'#12907F',min:9,fin:'Spur 1 sichern',blocks:[
 mis('Vergleiche Schädel und Gebiss von Mensch und Schimpanse. Die Antworten stehen nicht im Text, sondern in den Bildern und im Modell.'),
 H(fig2(skull('m'),'Schädel Mensch',skull('s'),'Schädel Schimpanse')),
 H(fig2(teeth('m'),'Oberkiefer Mensch, Draufsicht',teeth('s'),'Oberkiefer Schimpanse, Draufsicht')),
 {t:'task',id:'1.1',lvl:1,op:'Beschreibe',text:'bei beiden Schädeln das Größenverhältnis von Gehirnschädel (rosa) zu Gesichtsschädel (blau) und die Besonderheiten über den Augen. Nutze auch die Würfel zum Gehirnvolumen.',field:'Feld 3a',
  hints:['Welche Farbfläche ist jeweils größer?','Wie weit ragt das Gesicht nach vorne? Was liegt über dem Auge?'],
  sol:'Mensch: Gehirnschädel größer als Gesichtsschädel, Gehirn etwa dreimal so groß wie beim Schimpansen, keine kräftigen Wülste über den Augen. Schimpanse: Gesichtsschädel größer, schnauzenförmig, ausgeprägter Überaugenwulst.'},
 {t:'task',id:'1.2',lvl:1,op:'Vergleiche',text:'die beiden Zahnbögen: Form des Bogens, Länge der rötlichen Eckzähne und Auffälligkeiten zwischen den Zähnen. Zähle außerdem die Zähne im Oberkiefer. Wie viele hat dann das ganze Gebiss mit Unterkiefer?',field:'Feld 3c',
  hints:['Beschreibe die Form mit einem Buchstaben oder einer Figur.','Zähle jede Zeichnung einzeln. Der Unterkiefer hat genauso viele Zähne wie der Oberkiefer.'],
  sol:'Mensch: bogenförmig, kleine Eckzähne. Schimpanse: rechteckig, dolchartige Eckzähne, Lücke zwischen Schneide- und Eckzähnen. Beide 16 Zähne oben, also 32 Zähne insgesamt: Gemeinsamkeit.'},
 {t:'task',id:'1.3',lvl:2,op:'Untersuche',text:'mit dem Biss-Modell, ob sich der Kiefer in beiden Varianten ganz schließen lässt. Erkläre, wozu die Lücke im Unterkiefer bei langen oberen Eckzähnen nötig ist. Nenne außerdem eine Schwäche des Modells.',field:'Feld 3c (Folgerung)',w:{n:'bite'},
  hints:['Beobachte, wo die langen Zähne beim Schließen landen.','Was zeigt das Modell nicht, was beim echten Kauen wichtig wäre?'],
  sol:'Die langen oberen Eckzähne tauchen beim Schließen in den Unterkiefer ein. Ohne Lücke stoßen sie auf die unteren Zähne. Die Lücke bietet ihnen Platz. Schwäche: nur Seitenansicht, keine Kaubewegung, keine Muskeln.'},
 {t:'task',id:'1.4',lvl:3,star:1,op:'Stelle',text:'eine begründete Vermutung auf, welche Aufgabe der kräftige Überaugenwulst des Schimpansen haben könnte. Schimpansen fressen auch hartschalige Nahrung, zum Beispiel Nüsse. Denke an die Kräfte beim Kauen.',field:'Feld 3a (Folgerung)',
  hints:['Beim Knacken harter Schalen wirken große Kräfte auf den Schädel.','Wozu dienen Verdickungen und Verstärkungen bei Bauwerken?'],
  sol:'Der Wulst stabilisiert den Schädel beim Kauen hartschaliger Nahrung.'}]});

STATIONS.push({id:'s2',no:'SPUR 2',title:'Hinterhauptsloch: Wie trägt man einen Kopf?',teaser:'Modellversuch mit Knete und Stift.',c:'#12907F',min:9,fin:'Spur 2 sichern',blocks:[
 mis('An der Stelle des roten Punktes tritt die Wirbelsäule in den Schädel ein (Hinterhauptsloch). Finde heraus, was die Lage für den Kopf bedeutet.'),
 H(fig2(headspine('m'),'Mensch, Seitenansicht',headspine('s'),'Schimpanse, Seitenansicht')),
 {t:'task',id:'2.1',lvl:1,op:'Beschreibe',text:'die Lage des roten Punktes am Schädel und die Richtung der Wirbelsäule bei Mensch und Schimpanse.',field:'Feld 3b',
  hints:['Liegt der Punkt eher unter dem Schädel oder eher hinten? Wo liegt dann der Schädel im Verhältnis zur Wirbelsäule?'],
  sol:'Mensch: Hinterhauptsloch unter dem Schädel, der Kopf sitzt auf der Wirbelsäule. Schimpanse: im hinteren Bereich, der Kopf liegt vor der Wirbelsäule.'},
 {t:'task',id:'2.2',lvl:2,op:'Stelle',text:'eine Vermutung auf: Bei welcher Lage braucht man mehr Muskelkraft im Nacken, damit der Kopf nicht nach vorne kippt?',field:'Feld 4 (Vermutung)',w:{n:'poll',c:{key:'p2',opts:['Bei der Lage wie beim Menschen','Bei der Lage wie beim Schimpansen','Bei beiden gleich viel']}},
  hints:['Stelle dir vor, du balancierst einen Ball auf einem Stab. Wo musst du den Stab ansetzen, damit der Ball nicht kippt?'],sol:'Erwartet wird: beim Schimpansen. Der Kopf liegt vor der Wirbelsäule und zieht nach vorne.'},
 {t:'task',id:'2.3',lvl:2,op:'Führe',text:'den Modellversuch durch und notiere deine Beobachtungen. <div class="info"><b class="k">Material:</b> Bleistift, Knetmasse.<br><b class="k">1.</b> Forme einen Knetfuß und stelle den Bleistift senkrecht hinein (Wirbelsäule).<br><b class="k">2. Mensch-Modell:</b> Drücke eine Knetkugel (Kopf) so auf das obere Ende, dass der Stift mittig unter der Kugel sitzt. Bleibt sie von allein stehen?<br><b class="k">3. Schimpansen-Modell:</b> Befestige die Kugel so, dass der Stift hinten an der Kugel ansetzt und die Kugel nach vorne übersteht. Was passiert? Was müsste man tun, damit sie oben bleibt?</div>',field:'Feld 4 (Beobachtung)',
  hints:['Beschreibe beide Modelle nacheinander: stabil, wackelig, kippt?'],sol:'Erwartung (bitte vorab testen): Mensch-Modell steht fast von allein. Schimpansen-Modell kippt nach vorne; man müsste die Kugel von hinten festhalten oder stützen.'},
 {t:'task',id:'2.4',lvl:2,star:1,op:'Ordne',text:'zu, wofür die Modellteile im Original stehen.',field:'Feld 4',w:{n:'modelmap',c:{rows:[['Knetkugel',0],['Bleistift',1],['Festhalten der Kugel von hinten',2]],opts:['Schädel','Wirbelsäule','Nackenmuskulatur','Brustkorb']}},
  hints:['Überlege, was den Kopf trägt und was ihn hält.'],sol:'Knetkugel = Schädel, Bleistift = Wirbelsäule, Festhalten von hinten = Nackenmuskulatur.'},
 {t:'task',id:'2.5',lvl:3,op:'Erkläre',text:'mit dem Modell, warum Schimpansen eine starke Nackenmuskulatur brauchen, Menschen aber weniger. Beurteile außerdem das Modell: Nenne eine Stärke und eine Schwäche.',field:'Feld 4 (Deutung) und Feld 3b',
  hints:['Verwende die Zuordnung der Modellteile in deiner Erklärung.','Ist ein Kopf wirklich eine Kugel? Was fehlt dem Modell, das im Körper den Kopf hält?'],
  sol:'Beim Schimpansen liegt der Kopf vor der Wirbelsäule und zieht nach vorne, die starke Nackenmuskulatur hält ihn. Beim Menschen ruht der Kopf auf der Wirbelsäule, das braucht weniger Muskelkraft. Stärke des Modells: Kippneigung gut sichtbar. Schwäche: Kopf ist keine Kugel, die Nackenmuskulatur fehlt im Modell ganz.'}]});

STATIONS.push({id:'s3',no:'SPUR 3',title:'Wirbelsäule und Brustkorb',teaser:'Welche Form federt Stöße ab? Modellversuch mit dem Drahtmodell.',c:'#12907F',min:9,fin:'Spur 3 sichern',blocks:[
 mis('Beim Gehen, Laufen und Springen trifft jeder Schritt den Körper wie ein kleiner Stoß. Wie geht die Wirbelsäule damit um?'),
 H(fig2(spine('m'),'Wirbelsäule Mensch',spine('s'),'Wirbelsäule Schimpanse')),
 H(fig2(ribs('m'),'Brustkorb Mensch, Vorderansicht',ribs('s'),'Brustkorb Schimpanse, Vorderansicht')),
 {t:'task',id:'3.1',lvl:1,op:'Beschreibe',text:'die Form der Wirbelsäule und des Brustkorbs bei Mensch und Schimpanse.',field:'Feld 3d und 3e',
  hints:['Vergleiche die Wirbelsäulen mit einem Buchstaben. Den Brustkorb mit einem Körper aus dem Alltag.'],sol:'Mensch: Wirbelsäule doppelt S-förmig, Brustkorb tonnenförmig. Schimpanse: Wirbelsäule C-förmig, Brustkorb kegelförmig (oben schmal, unten breit).'},
 {t:'task',id:'3.2',lvl:2,op:'Stelle',text:'eine Vermutung auf: Welche Form gibt bei einem Stoß von oben am ehesten federnd nach und kehrt danach zurück?',field:'Feld 5 (Vermutung)',w:{n:'poll',c:{key:'p3',opts:['gerader Stab','C-Form','doppelte S-Form']}},
  hints:['Denke an eine Sprungfeder oder einen Skistock, der sich durchbiegt.'],sol:'Erwartet wird die doppelte S-Form. Das Experiment zeigt, ob die Vermutung stimmt.'},
 {t:'task',id:'3.3',lvl:2,op:'Untersuche',text:'im Modellversuch drei Formen. <div class="info"><b class="k">Material:</b> das vorbereitete Drahtmodell am Materialtisch.<br><b class="k">1.</b> Draht gerade, <b class="k">2.</b> Draht in C-Form, <b class="k">3.</b> Draht in doppelter S-Form.<br>Halte das Modell unten fest und drücke mit der Fingerspitze langsam von oben. Beobachte: Wie weit gibt es nach? Wie verformt es sich? Kehrt es zurück? Biege den Draht nach dem Versuch wieder in die Ausgangsform.</div>',field:'Feld 5 (Tabelle)',
  hints:['Halte die Kraft bei allen drei Formen ungefähr gleich. Warum ist das wichtig für einen fairen Vergleich?'],sol:'Erwartung (mit dem Drahtmodell vorab testen): gerade starr, C-Form knickt nach vorne durch, S-Form gibt federnd nach und kehrt zurück. Variablen: Draht, Länge, Kraft gleich halten; nur die Form ändern.'},
 {t:'task',id:'3.4',lvl:2,op:'Erkläre',text:'mit deinen Beobachtungen, warum die doppelte S-Form für ein Lebewesen wichtig ist, das bei jedem Schritt und Sprung Stöße erfährt. Was stellt der Druck von oben im Modell dar?',field:'Feld 5 (Erklärung) und Feld 3d',
  hints:['Wohin geht ein Stoß bei der geraden Form? Wohin bei der S-Form?'],sol:'Der Druck steht für den Stoß beim Auftreten. Die S-Form gibt federnd nach und fängt Stöße und Erschütterungen ab. Das schützt Wirbel und Kopf beim aufrechten Gehen und Springen.'},
 {t:'task',id:'3.5',lvl:2,op:'Ordne',text:'die Bewegungen dem passenden Brustkorb zu und begründe mit der Form: Wo bleibt oben bei schmalem Brustkorb Platz um die Schultergelenke?',field:'Feld 3e (Folgerung)',w:{n:'assign',c:{key:'s35',opts:['tonnenförmiger Brustkorb','kegelförmiger Brustkorb'],items:[['Oberkörper beim Aufrechtgehen nach vorne beugen, um etwas aufzuheben',0],['Arme weit seitlich und nach oben bewegen, um sich im Geäst zu hangeln',1]]}},
  hints:['Wo sitzen die Schultergelenke im Verhältnis zum Brustkorb?'],sol:'Tonnenförmig: Oberkörper kann gebeugt werden. Kegelförmig: oben schmal, die Schultergelenke haben viel Bewegungsfreiheit, passend zum Klettern und Hangeln.'}]});
/* ===== Stationen 4 bis 6 und Transfer ===== */
STATIONS.push({id:'s4',no:'SPUR 4',title:'Becken und Gliedmaßen',teaser:'Rechnen mit Körperproportionen und ein Balance-Modell.',c:'#12907F',min:9,fin:'Spur 4 sichern',blocks:[
 mis('Becken, Arme und Beine bestimmen, wie ein Körper steht und sich fortbewegt. Du rechnest und testest ein Modell.'),
 H(fig2(pelvis('m'),'Becken Mensch, Vorderansicht',pelvis('s'),'Becken Schimpanse, Vorderansicht')),
 H(fig2(figure('m'),'Körperproportionen Mensch',figure('s'),'Körperproportionen Schimpanse')+'<div class="note">Die Längen sind Schemawerte in Einheiten, keine echten Messwerte.</div>'),
 {t:'task',id:'4.1',lvl:1,op:'Beschreibe',text:'die Form der beiden Becken in Breite, Länge und Wölbung.',field:'Feld 3f',
  hints:['Vergleiche Breite und Höhe jeweils miteinander. Welche Form erinnert an eine Schale oder Schaufel?'],sol:'Mensch: schaufelförmig, breiter, kippbar. Schimpanse: länger, schmaler, nach vorne gekippt.'},
 {t:'task',id:'4.2',lvl:2,op:'Berechne',text:'für beide Figuren das Verhältnis Armlänge geteilt durch Beinlänge (zwei Stellen nach dem Komma) und vergleiche die Werte mit der Zahl 1.',field:'Feld 3g',w:{n:'ratio',c:{a:0.70,b:1.5454}},
  hints:['Mensch: Arm geteilt durch Bein. Ein Wert unter 1 bedeutet, dass die Arme kürzer sind als die Beine.'],sol:'Mensch 70 : 100 = 0,70, Schimpanse 85 : 55 = 1,55. Beim Menschen sind die Arme kürzer als die Beine, beim Schimpansen länger.'},
 {t:'task',id:'4.3',lvl:2,op:'Untersuche',text:'mit dem Balance-Modell, wo das rote Lot jeweils auftrifft. Erkläre, warum ein Schimpanse, der aufrecht auf zwei Beinen steht, leichter nach vorne kippt als ein Mensch. Beziehe die Wirbelsäule ein.',field:'Feld 3d und 3f (Folgerung)',w:{n:'balance'},
  hints:['Ein Körper steht stabil, solange das Lot des Schwerpunkts auf die Standfläche trifft.','Erinnere dich an die Form der Wirbelsäule und an die Lage des Körperschwerpunkts.'],
  sol:'Beim Schimpansen liegt der Körperschwerpunkt wegen der C-förmigen Wirbelsäule weiter vorne. Das Lot fällt vor die Füße, er kippt nach vorne. Beim Menschen liegt der Schwerpunkt über den Füßen. Das Becken muss zur Körperhaltung passen. Das Modell ist ein stark vereinfachtes Schema.'},
 {t:'task',id:'4.4',lvl:3,star:1,op:'Leite',text:'aus Armlänge, Beckenform und Wirbelsäule ab, wie sich Schimpansen am Boden und in Bäumen fortbewegen, und begründe.',field:'Feld 3g (Folgerung)',
  hints:['Wie weit reichen lange Arme? Was hilft dem Körper beim Gehen mit vorverlagertem Schwerpunkt?'],sol:'Lange Arme, ein nach vorne gekipptes Becken und eine C-förmige Wirbelsäule passen zum Laufen auf allen Vieren und zum Klettern: Die Arme stützen den Körper und reichen weit zu Ästen.'}]});

STATIONS.push({id:'s5',no:'SPUR 5',title:'Hand und Fuß',teaser:'Selbstversuch mit Stoppuhr: Was kann dein Daumen?',c:'#12907F',min:9,fin:'Spur 5 sichern',blocks:[
 mis('Vergleiche Hände und Füße im Bild. Danach testest du an dir selbst, wie wichtig der Daumen ist.'),
 H(fig2(hand('m'),'Hand Mensch',hand('s'),'Hand Schimpanse')),
 H(fig2(foot('m'),'Fuß Mensch',foot('s'),'Fuß Schimpanse')),
 {t:'task',id:'5.1',lvl:1,op:'Vergleiche',text:'Hände und Füße im Bild. Beachte die Stellung von Daumen und großem Zeh. Nenne eine Gemeinsamkeit und einen Unterschied.',field:'Feld 3h und 3i',
  hints:['Kann man den Daumen jeweils den anderen Fingern gegenüberstellen? Und den großen Zeh den anderen Zehen?'],
  sol:'Hand: Bei beiden lässt sich der Daumen den Fingern gegenüberstellen (opponierbar, Pinzettengriff), beide haben Fingernägel: Gemeinsamkeit. Fuß: Beim Menschen zeigt der große Zeh nach vorne, beim Schimpansen ist er opponierbar (Greiffuß).'},
 {t:'task',id:'5.2',lvl:2,op:'Führe',text:'den Selbstversuch durch. Eine Person fixiert den Daumen der Schreibhand locker mit Klebeband an der Handfläche (nicht abschnüren, bei Kribbeln sofort lösen). <b>Vermute zuerst</b>, um welchen Faktor es länger dauert. Messt dann mit der Stoppuhr erst mit, dann ohne Daumen: <b>(1)</b> Münze vom Tisch aufheben, <b>(2)</b> Knopf schließen, <b>(3)</b> den eigenen Namen schreiben. Trage die Zeiten ein.',field:'Feld 6 (Messwerte)',w:{n:'stopwatch'},
  hints:['Variablen: Was bleibt gleich, was wird verändert? Wiederholt jede Messung, um Zufall zu verringern.'],sol:'Messwerte sind individuell. Ohne Daumen dauert jede Aufgabe deutlich länger. Konstant: Person, Aufgabe, Hand. Variabel: Daumen frei oder fixiert.'},
 {t:'task',id:'5.3',lvl:2,op:'Berechne',text:'für jede Aufgabe den Faktor (Zeit ohne Daumen geteilt durch Zeit mit Daumen) und interpretiere: Was sagt dein Ergebnis zur Bedeutung des Daumens? Verbinde es mit deinem Handvergleich aus 5.1.',field:'Feld 6 (Faktor, Deutung)',
  hints:['Ein Faktor über 1 bedeutet: ohne Daumen dauert es länger.','Wenn beide Arten diesen Daumen besitzen: Spricht das eher für Verwandtschaft oder dagegen?'],
  sol:'Faktor deutlich größer als 1: Der gegenüberstellbare Daumen ermöglicht den Pinzettengriff und feine Arbeit. Schimpansen haben ihn ebenfalls: eine Gemeinsamkeit, die für Verwandtschaft spricht.'},
 {t:'task',id:'5.4',lvl:3,op:'Leite',text:'her, wozu welcher Fuß besser passt. Der große Zeh des Schimpansen lässt sich wie ein Daumen gegenüberstellen, der des Menschen zeigt nach vorne. Begründe für Gehen und für Klettern. Freiwillig: Versuche, einen Stift mit den Zehen zu greifen.',field:'Feld 3i (Folgerung)',
  hints:['Womit kann man Äste umfassen? Was braucht ein Fuß, der den Körper beim Gehen abrollt und trägt?'],sol:'Mensch: nach vorne gerichteter großer Zeh bildet einen Standfuß zum Stehen und Gehen. Schimpanse: opponierbarer großer Zeh ist ein Greiffuß, der Äste umfassen kann.'}]});

const ITEMS61=[['Form der Wirbelsäule',1],['Skelett aus Schädel, Wirbelsäule, Brustkorb, Becken, Armen und Beinen',0],['Lage des Hinterhauptslochs',1],['Stellung des großen Zehs',1],['gleiche Zahl an Zähnen: 32',0],['Größe des Gehirns',1],['Daumen lässt sich den Fingern gegenüberstellen, Fingernägel',0],['Armlänge im Vergleich zur Beinlänge',1],['Mimik, Gestik und Fürsorge für den Nachwuchs',0],['Form des Beckens',1]];
STATIONS.push({id:'s6',no:'SPUR 6',title:'Auswertung: Beweisaufnahme',teaser:'Ergebnisse zusammenführen, Hypothese prüfen, Stammbaum bauen.',c:'#6C4AB6',min:15,fin:'Fall abschließen',blocks:[
 {t:'fn',f:()=>`<div class="info"><b class="k">Deine Hypothese vom Anfang:</b> ${S.hyp?`<b>${S.hyp}</b> ${HYP[S.hyp]}`:'noch keine festgehalten'}</div>`},
 mis('Du hast fünf Spuren gesichert. Jetzt entscheidet die Beweislage, nicht die Meinung.'),
 {t:'task',id:'6.1',lvl:1,op:'Ordne',text:'die Beobachtungen aus deiner Tabelle (Feld 3) den Gemeinsamkeiten oder den Unterschieden zu.',field:'Feld 3 (Überblick)',w:{n:'assign',c:{key:'s61',opts:['Gemeinsamkeit','Unterschied'],items:ITEMS61}},
  hints:['Schau in deine Tabelle: Wo steht in beiden Spalten dasselbe?'],sol:'Gemeinsamkeiten: Skelettbau, 32 Zähne, Daumen und Fingernägel, Verhalten. Unterschiede: Wirbelsäule, Hinterhauptsloch, Arm-Bein-Verhältnis, großer Zeh, Becken, Gehirngröße.'},
 {t:'task',id:'6.2',lvl:2,op:'Ordne',text:'die Unterschiede der Anpassung zu, zu der sie passen. Ergänze danach die Spalte „Folgerung“ in Feld 3, falls dort noch etwas fehlt.',field:'Feld 3 (Folgerung)',w:{n:'assign',c:{key:'s62',opts:['aufrechter Gang','Klettern, Laufen auf allen Vieren'],items:[['Arme länger als Beine',1],['Hinterhauptsloch unter dem Schädel',0],['Greiffuß',1],['schaufelförmiges, kippbares Becken',0],['C-förmige Wirbelsäule',1],['großer Zeh nach vorne gerichtet',0],['doppelt S-förmige Wirbelsäule',0],['langes, schmales, nach vorne gekipptes Becken',1]]}},
  hints:['Wende an, was du in den Spuren herausgefunden hast: Stoßdämpfung, Kopfbalance, Schwerpunkt.'],sol:'Aufrechter Gang: S-Wirbelsäule, Hinterhauptsloch unten, schaufelförmiges Becken, Standfuß. Klettern und Laufen auf allen Vieren: C-Wirbelsäule, langes Becken, lange Arme, Greiffuß.'},
 {t:'task',id:'6.3',lvl:3,op:'Prüfe',text:'deine Hypothese: Welche der Hypothesen H1, H2 oder H3 stützen deine Ergebnisse? Begründe mit mindestens zwei Beobachtungen aus Feld 3. Nimm Stellung: Musst du deine Hypothese ändern? Wenn ja, warum?',field:'Feld 7',
  hints:['Was folgt aus den vielen Gemeinsamkeiten für H3?','Auch der heutige Schimpanse hat sich über lange Zeit verändert. Welche Merkmale sind bei ihm besonders ausgeprägt?'],
  sol:'H2 wird gestützt. Gemeinsamkeiten (Skelettbau, Zähne, Daumen) widerlegen H3. Die Unterschiede sind Anpassungen an verschiedene Lebensweisen; auch der heutige Schimpanse hat eigene Spezialisierungen (Greiffuß, lange Arme) und ist kein unveränderter Vorfahr. Das spricht gegen H1. Wer H1 oder H3 gewählt hat, ändert die Hypothese. Das gehört zur Wissenschaft.'},
 {t:'task',id:'6.4',lvl:3,op:'Übertrage',text:'das Modell Familienstammbaum: Zwei Cousinen haben dieselben Großeltern, stammen aber nicht voneinander ab. Ordne die Felder A, B, C im Stammbaum zu. Beurteile das Modell: Nenne eine Stärke und eine Schwäche.',field:'Feld 8',w:{n:'treeassign'},
  hints:['Wer steht im Familienstammbaum unten an der Wurzel, wer oben an den Ästen?','Was kann ein Familienstammbaum nicht zeigen, wenn es um sehr lange Zeiträume und Arten geht?'],
  sol:'A und B: Mensch und Schimpanse, C: gemeinsame Vorfahren. Stärke: zeigt Verzweigung und gemeinsame Vorfahren, ein Cousin stammt nicht vom anderen ab. Schwäche: Millionen Jahre und ganze Arten lassen sich nicht wie Personen darstellen.'},
 {t:'task',id:'6.5',lvl:2,op:'Formuliere',text:'in eigenen Worten eine Antwort auf die Frage „Stammt der Mensch vom Affen ab?“ und fülle danach den Lückentext in Feld 7 mit dem Wortspeicher aus.',field:'Feld 7 (Lückentext)',
  hints:['Verwende die Wörter Gemeinsamkeiten, Anpassungen, gemeinsame Vorfahren und nicht.'],sol:'Mensch und Schimpanse zeigen viele Gemeinsamkeiten in Körperbau und Verhalten. Die Unterschiede sind Anpassungen an Gehen oder Klettern. Beide haben gemeinsame Vorfahren, stammen aber nicht direkt voneinander ab.'}]});

STATIONS.push({id:'t1',no:'TRANSFER T1',title:'Fund X: Wer ist das?',teaser:'Ein Skelett mit gemischten Merkmalen. Beurteile Lebensweise und Bedeutung.',c:'#3E8E41',min:15,opt:1,fin:'Aufgabe sichern',blocks:[
 H(`<div class="info"><b class="k">Hinweis:</b> Fund X ist ein erfundener Fall für diese Aufgabe, kein echter Fossilfund.<br><br>Bei einer Ausgrabung wird ein Skelett von Fund X untersucht. Der Bericht nennt: Schnauzenförmiges Gesicht mit kräftigem Überaugenwulst. Wirbelsäule doppelt S-förmig. Zahnbogen rechteckig mit Lücke. Hinterhauptsloch weit unter dem Schädel. Gehirnschädel klein, Gesichtsschädel größer. Becken breit und schaufelförmig.</div>`),
 {t:'task',id:'T1.1',lvl:2,op:'Ordne',text:'jedes Merkmal von Fund X als eher menschenähnlich oder eher schimpansenähnlich ein.',field:'Feld 9',w:{n:'assign',c:{key:'t11',opts:['menschenähnlich','schimpansenähnlich'],items:[['kräftiger Überaugenwulst, schnauzenförmiges Gesicht',1],['doppelt S-förmige Wirbelsäule',0],['rechteckiger Zahnbogen mit Lücke',1],['Hinterhauptsloch weit unter dem Schädel',0],['kleiner Gehirnschädel, größerer Gesichtsschädel',1],['breites, schaufelförmiges Becken',0]]}},
  hints:['Vergleiche mit deiner Tabelle aus Feld 3.'],sol:'Menschenähnlich: Hinterhauptsloch, S-Wirbelsäule, Becken. Schimpansenähnlich: Schädelproportion, Überaugenwulst, Zahnbogen.'},
 {t:'task',id:'T1.2',lvl:3,op:'Beurteile',text:'wie sich Fund X wahrscheinlich fortbewegt hat. Begründe mit mindestens zwei Merkmalen.',field:'Feld 9',
  hints:['Welche Merkmale gehören zur Anpassung an den aufrechten Gang?'],sol:'Wahrscheinlich aufrechter Gang: Hinterhauptsloch unten (Kopf balanciert), S-Wirbelsäule (Stoßdämpfung), breites Becken (Körperhaltung).'},
 {t:'task',id:'T1.3',lvl:3,op:'Erkläre',text:'was ein Fund mit Merkmalen beider Gruppen für die Frage „Stammt der Mensch vom Affen ab?“ bedeutet. Warum passt er besser zu gemeinsamen Vorfahren als zu einem plötzlichen Sprung vom Affen zum Menschen?',field:'Feld 9',
  hints:['Entstehen alle Merkmale eines Lebewesens gleichzeitig oder nacheinander?'],sol:'Ein Mosaik aus menschen- und affenähnlichen Merkmalen zeigt, dass Merkmale nicht alle gleichzeitig entstanden sind. Das passt zu schrittweiser Entwicklung aus gemeinsamen Vorfahren. (Vorgriff auf Mosaikformen im Lernbereich Evolution.)'}]});

STATIONS.push({id:'t2',no:'TRANSFER T2',title:'Bionik: Die Roboter-Ingenieure',teaser:'Baue gedanklich zwei Roboter nach Vorbildern aus der Natur.',c:'#3E8E41',min:15,opt:1,fin:'Aufgabe sichern',blocks:[
 H(`<div class="info">Ein Ingenieurteam plant zwei Roboter für Katastrophengebiete. <b>Roboter A</b> soll aufrecht auf zwei Beinen über unebenen Boden gehen und Stöße abfedern. <b>Roboter B</b> soll in Gerüsten und Trümmern klettern und Dinge greifen. Bionik bedeutet: Technik nach Vorbildern aus der Natur.</div>`),
 {t:'task',id:'T2.1',lvl:3,op:'Entwirf',text:'Roboter A: Wähle drei Merkmale des Menschen aus Feld 3 aus und begründe jede Wahl mit einer Funktion.',field:'Feld 9',
  hints:['Stoßdämpfung, Kopfbalance, sicherer Stand: Welches Merkmal leistet was?'],sol:'Mögliche Wahl: S-förmige Wirbelsäule (federt Stöße ab), breites schaufelförmiges Becken (Haltung), nach vorne gerichteter Standfuß (Stand und Abrollen), Kopf mittig auf der Wirbelsäule (wenig Haltekraft).'},
 {t:'task',id:'T2.2',lvl:3,op:'Übertrage',text:'Merkmale des Schimpansen auf Roboter B: Wähle drei Merkmale aus und begründe.',field:'Feld 9',
  hints:['Wie reicht man weit? Wie hält man sich fest?'],sol:'Mögliche Wahl: lange Arme (große Reichweite), Greiffuß (Äste und Streben umfassen), kegelförmiger Brustkorb (bewegliche Schultergelenke), Gliedmaßen für Fortbewegung auf allen Vieren.'},
 {t:'task',id:'T2.3',lvl:3,op:'Beurteile',text:'die Grenzen des Vorbilds Natur: Nenne zwei Punkte, in denen ein Roboter nicht wie ein Lebewesen funktioniert.',field:'Feld 9',
  hints:['Denke an Material, Energie und Steuerung.'],sol:'Z. B. Metall und Motoren statt Knochen und Muskeln, Energie aus Akku statt Nahrung, Steuerung durch Programme statt Nervensystem, kein Wachstum und keine Reparatur.'}]});

STATIONS.push({id:'t3',no:'TRANSFER T3',title:'Rückencheck im Schulalltag',teaser:'Wende das Wissen über die S-Form auf dein eigenes Verhalten an.',c:'#3E8E41',min:15,opt:1,fin:'Aufgabe sichern',blocks:[
 H(`<div class="info"><b>Drei Alltagssituationen:</b><br>(1) Eine schwere Schultasche wird an einem Träger über einer Schulter getragen.<br>(2) Eine Schülerin sitzt stundenlang mit rundem Rücken vor dem Bildschirm.<br>(3) Ein Schüler landet nach einem Sprung vom Kasten mit durchgestreckten Beinen.</div>`),
 {t:'task',id:'T3.1',lvl:3,op:'Beurteile',text:'für jede Situation, wie sie zur Funktion der doppelten S-Form der Wirbelsäule passt oder ihr entgegenwirkt. Entscheide, welche Situation du für am belastendsten hältst, und begründe.',field:'Feld 9',
  hints:['Die S-Form federt Stöße ab. Was passiert, wenn der Stoß nicht gedämpft wird oder die Form verändert wird?'],
  sol:'(1) Einseitige Last belastet die Wirbelsäule ungleich. (2) Rundrücken weicht von der natürlichen S-Form ab, die Dämpfung wird schlechter genutzt. (3) Gestreckte Beine geben den Stoß fast ungedämpft in die Wirbelsäule weiter. Begründete Gewichtung ist wichtiger als die Wahl selbst.'},
 {t:'task',id:'T3.2',lvl:3,op:'Entwickle',text:'drei Regeln für rückenfreundliches Verhalten im Schulalltag und begründe jede mit der Funktion der Wirbelsäule.',field:'Feld 9',
  hints:['Tragen, Sitzen, Springen: Eine Regel pro Bereich.'],sol:'Z. B. Tasche auf beiden Schultern und nah am Körper tragen; aufrecht sitzen und zwischendurch bewegen; Sprünge mit gebeugten Knien abfedern. Jeweils mit Bezug auf die Dämpfung durch die S-Form.'}]});

renderHome();
</script></body></html>
