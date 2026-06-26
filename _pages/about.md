---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Hi, I'm a second year graduate student at ShanghaiTech University. My current research focus in Deep Generative Models, such as Diffusion Bridge and Flow Matching.

I am a National Master of Sport in Chess, certified by the Chinese Chess Association.

<div class="kz-chess" id="kzChess">
<style>
.kz-chess{position:relative;margin:26px 0;padding:22px;border-radius:20px;background:linear-gradient(135deg,#1b2440 0%,#2a3a66 45%,#3b2c63 100%);box-shadow:0 18px 50px -12px rgba(20,24,60,.65),inset 0 1px 0 rgba(255,255,255,.08);color:#eef1fb;overflow:hidden;}
.kz-chess::before{content:"";position:absolute;inset:-45%;background:conic-gradient(from 0deg,transparent 0 68%,rgba(120,170,255,.35) 80%,transparent 92%);animation:kzspin 9s linear infinite;z-index:0;pointer-events:none;}
@keyframes kzspin{to{transform:rotate(360deg);}}
.kz-chess__inner{position:relative;z-index:1;display:flex;flex-wrap:wrap;gap:22px;align-items:flex-start;}
.kz-board-wrap{flex:0 0 auto;width:min(360px,86vw);}
.kz-board{position:relative;width:100%;aspect-ratio:1/1;border-radius:10px;background:#e9edf8;box-shadow:0 10px 30px -8px rgba(0,0,0,.55),inset 0 0 0 3px rgba(255,255,255,.14);font-size:34px;overflow:hidden;}
.kz-cells{position:absolute;inset:0;z-index:0;display:grid;grid-template-columns:repeat(8,1fr);grid-template-rows:repeat(8,1fr);}
.kz-cell--d{background:#5d77bd;box-shadow:0 0 0 .5px #5d77bd;}
.kz-cell--l{background:#e9edf8;box-shadow:0 0 0 .5px #e9edf8;}
.kz-piece{position:absolute;left:0;top:0;width:12.5%;height:12.5%;display:flex;align-items:center;justify-content:center;font-size:1em;line-height:1;z-index:3;pointer-events:none;transition:left .45s cubic-bezier(.22,.61,.36,1),top .45s cubic-bezier(.22,.61,.36,1);will-change:left,top;}
.kz-noanim .kz-piece,.kz-noanim .kz-hl{transition:none!important;}
.kz-w{color:#f6f8fc;text-shadow:-1px -1px 0 #2b3140,1px -1px 0 #2b3140,-1px 1px 0 #2b3140,1px 1px 0 #2b3140,0 3px 4px rgba(0,0,0,.45);}
.kz-b{color:#161a24;text-shadow:-1px -1px 0 rgba(255,255,255,.5),1px -1px 0 rgba(255,255,255,.5),-1px 1px 0 rgba(255,255,255,.5),1px 1px 0 rgba(255,255,255,.5),0 3px 4px rgba(0,0,0,.4);}
.kz-cap{animation:kzcap .42s forwards;z-index:2;}
@keyframes kzcap{to{opacity:0;transform:scale(.12) rotate(40deg);}}
.kz-hl{position:absolute;left:0;top:0;width:12.5%;height:12.5%;z-index:1;pointer-events:none;border-radius:5px;background:rgba(255,201,64,.42);box-shadow:0 0 16px rgba(255,201,64,.55);opacity:0;transition:left .45s cubic-bezier(.22,.61,.36,1),top .45s cubic-bezier(.22,.61,.36,1),opacity .25s;}
.kz-hl--to{animation:kzpulse 1s ease-in-out infinite;}
@keyframes kzpulse{0%,100%{box-shadow:0 0 12px rgba(255,201,64,.5);}50%{box-shadow:0 0 24px rgba(255,201,64,.95);}}
.kz-coord{position:absolute;font:700 9px/1 system-ui,Arial,sans-serif;color:rgba(15,22,40,.5);z-index:2;pointer-events:none;}
.kz-coord--f{bottom:2px;text-align:right;padding-right:3px;}
.kz-coord--r{left:3px;top:0;padding-top:2px;}
.kz-controls{display:flex;gap:8px;justify-content:center;flex-wrap:wrap;margin-top:13px;}
.kz-controls button{cursor:pointer;border:1px solid rgba(255,255,255,.22);background:rgba(255,255,255,.08);color:#eef1fb;font-size:15px;line-height:1;min-width:42px;padding:9px 12px;border-radius:11px;transition:transform .15s,background .2s,box-shadow .2s;}
.kz-controls button:hover{background:rgba(120,170,255,.3);transform:translateY(-2px);box-shadow:0 6px 16px -4px rgba(120,170,255,.6);}
.kz-controls button:active{transform:translateY(0);}
.kz-side{flex:1 1 240px;min-width:228px;}
.kz-title{margin:2px 0 10px;font-family:Georgia,serif;font-size:21px;color:#fff;text-shadow:0 2px 12px rgba(120,170,255,.55);}
.kz-status{font-size:13px;opacity:.85;margin-bottom:12px;letter-spacing:.3px;}
.kz-status b{color:#9fc0ff;font-size:15px;}
.kz-moves{position:relative;display:flex;flex-wrap:wrap;gap:6px;max-height:232px;overflow:auto;padding:4px;}
.kz-chip{cursor:pointer;border:none;font:600 12px/1 'Courier New',monospace;padding:6px 9px;border-radius:7px;outline:2px solid transparent;transition:transform .15s,box-shadow .2s,outline-color .2s;}
.kz-chip--w{background:#eef2fb;color:#1b2440;box-shadow:0 2px 5px rgba(0,0,0,.3);}
.kz-chip--b{background:#212a44;color:#dfe6fb;box-shadow:0 2px 5px rgba(0,0,0,.4),inset 0 0 0 1px rgba(255,255,255,.12);}
.kz-chip:hover{transform:translateY(-2px);}
.kz-chip.kz-on{outline-color:#5fd0ff;box-shadow:0 0 0 2px rgba(95,208,255,.5),0 0 16px rgba(95,208,255,.7);transform:translateY(-2px) scale(1.06);}
.kz-legend{margin-top:12px;font-size:11px;opacity:.78;display:flex;align-items:center;flex-wrap:wrap;gap:4px;}
.kz-dot{display:inline-block;width:11px;height:11px;border-radius:3px;margin-right:3px;vertical-align:-1px;}
.kz-dot--w{background:#eef2fb;}
.kz-dot--b{background:#212a44;border:1px solid rgba(255,255,255,.3);}
@media (max-width:560px){.kz-board-wrap{width:100%;}.kz-chess__inner{gap:16px;}}
/* ===== page-wide flair (applies live) ===== */
.page__content h1{position:relative;padding-bottom:6px;}
.page__content h1::after{content:"";position:absolute;left:0;bottom:0;height:3px;width:64px;border-radius:3px;background:linear-gradient(90deg,#6a4fb3,#3aa0c9);box-shadow:0 0 12px rgba(106,79,179,.6);transition:width .4s ease;}
.page__content h1:hover::after{width:120px;}
.paper-box{border-radius:12px;transition:transform .28s cubic-bezier(.22,.61,.36,1),box-shadow .28s;will-change:transform;}
.paper-box:hover{transform:translateY(-5px);box-shadow:0 16px 38px -14px rgba(42,58,102,.55);}
.paper-box-image img{transition:transform .35s ease,box-shadow .35s ease;border-radius:8px;}
.paper-box:hover .paper-box-image img{transform:scale(1.04);box-shadow:0 10px 26px -8px rgba(58,160,201,.5);}
.badge{background:linear-gradient(135deg,#2a3a66,#6a4fb3)!important;color:#fff!important;box-shadow:0 4px 12px -3px rgba(106,79,179,.6);letter-spacing:.3px;}
#about-me ~ p a,.paper-box-text a{transition:color .2s,text-shadow .2s;}
.paper-box-text a:hover{text-shadow:0 0 10px rgba(58,160,201,.55);}
#-news + ul li,#-honors-and-awards + ul li{transition:transform .2s,color .2s;border-radius:6px;padding-left:2px;}
#-news + ul li:hover,#-honors-and-awards + ul li:hover{transform:translateX(6px);color:#2a3a66;}
.author__avatar img{transition:transform .4s ease,box-shadow .4s ease;}
.author__avatar img:hover{transform:scale(1.05) rotate(-1deg);box-shadow:0 10px 28px -8px rgba(106,79,179,.6);}
@keyframes kzfadeup{from{opacity:0;transform:translateY(18px);}to{opacity:1;transform:translateY(0);}}
.paper-box{animation:kzfadeup .6s both;}
</style>
<div class="kz-chess__inner">
<div class="kz-board-wrap">
<div class="kz-board" id="kzBoard"></div>
<div class="kz-controls" id="kzCtl">
<button data-act="restart" title="Restart">&#10227;</button>
<button data-act="prev" title="Previous move">&#9198;</button>
<button data-act="play" id="kzPlay" title="Play / Pause">&#10074;&#10074;</button>
<button data-act="next" title="Next move">&#9197;</button>
<button data-act="flip" title="Flip board">&#8645;</button>
<button data-act="speed" id="kzSpeed" title="Playback speed">1&#215;</button>
</div>
</div>
<div class="kz-side">
<h3 class="kz-title">&#9819; My Chess Game</h3>
<div class="kz-status">Move <b id="kzPly">0</b> / 17 &middot; <span id="kzTurn">Black to move</span></div>
<div class="kz-moves" id="kzMoves"></div>
<div class="kz-legend"><span class="kz-dot kz-dot--w"></span>White<span style="width:8px"></span><span class="kz-dot kz-dot--b"></span>Black<span style="width:8px"></span>&middot; auto-playing &middot; click a move to jump</div>
</div>
</div>
<script>
(function(){
var START="r2q3k/pb3prp/1pn1pN2/8/2BP3Q/1P6/PBP3PP/R6K";
var UCI=["c6e5","d4d5","e6d5","b2e5","d5c4","h4h6","d8e7","f6g4","b7g2","h1g1","e7c5","h6e3","c5e3","g4e3","g2e4","e5g7","h8g7"];
var SAN=["Ne5","d5","exd5","Bxe5","dxc4","Qh6","Qe7","Ng4","Bg2","Kg1","Qc5","Qe3","Qxe3","Nxe3","Be4","Bxg7","Kxg7"];
var GLYPH={p:"♟",n:"♞",b:"♝",r:"♜",q:"♛",k:"♚"};
var board=document.getElementById("kzBoard");
if(!board){return;}
var pos={},flip=true,ply=0,playing=true,timer=null,curHL=null;
var SPEEDS=[900,1500,550],spi=0;
var cells=document.createElement("div");cells.className="kz-cells";for(var ci=0;ci<64;ci++){var cell=document.createElement("div");var rr=Math.floor(ci/8),cc=ci%8;cell.className="kz-cell--"+(((rr+cc)%2===0)?"l":"d");cells.appendChild(cell);}board.appendChild(cells);
var movesEl=document.getElementById("kzMoves");
var hlFrom=document.createElement("div");hlFrom.className="kz-hl";board.appendChild(hlFrom);
var hlTo=document.createElement("div");hlTo.className="kz-hl kz-hl--to";board.appendChild(hlTo);
var fileLabs=[],rankLabs=[];
for(var qi=0;qi<8;qi++){var fl=document.createElement("div");fl.className="kz-coord kz-coord--f";fl.style.width="12.5%";board.appendChild(fl);fileLabs.push(fl);var rl=document.createElement("div");rl.className="kz-coord kz-coord--r";rl.style.height="12.5%";board.appendChild(rl);rankLabs.push(rl);}
function frToCoord(f,r){var col=flip?7-f:f;var row=flip?r:7-r;return{x:col*12.5,y:row*12.5};}
function coord(sq){return frToCoord(sq.charCodeAt(0)-97,sq.charCodeAt(1)-49);}
function place(el,sq){var c=coord(sq);el.style.left=c.x+"%";el.style.top=c.y+"%";}
function relabel(){for(var f=0;f<8;f++){var col=flip?7-f:f;var e=fileLabs[f];e.textContent=String.fromCharCode(97+f);e.style.left=(col*12.5)+"%";}for(var r=0;r<8;r++){var row=flip?r:7-r;var e2=rankLabs[r];e2.textContent=(r+1);e2.style.top=(row*12.5)+"%";}}
function parseFEN(fen){var rows=fen.split("/");var p={};for(var r=0;r<8;r++){var rank=7-r,fi=0,row=rows[r];for(var k=0;k<row.length;k++){var ch=row[k];if(ch>="1"&&ch<="8"){fi+=parseInt(ch,10);}else{var color=(ch===ch.toUpperCase())?"w":"b";var sq=String.fromCharCode(97+fi)+String.fromCharCode(49+rank);p[sq]={type:ch.toLowerCase(),color:color};fi++;}}}return p;}
function makePiece(pc){var d=document.createElement("div");d.className="kz-piece kz-"+pc.color;d.textContent=GLYPH[pc.type];return d;}
function showHL(from,to){curHL=[from,to];var a=coord(from),b=coord(to);hlFrom.style.left=a.x+"%";hlFrom.style.top=a.y+"%";hlTo.style.left=b.x+"%";hlTo.style.top=b.y+"%";hlFrom.style.opacity=1;hlTo.style.opacity=1;}
function hideHL(){curHL=null;hlFrom.style.opacity=0;hlTo.style.opacity=0;}
function rebuild(){var olds=board.querySelectorAll(".kz-piece");for(var i=0;i<olds.length;i++){olds[i].remove();}pos=parseFEN(START);board.classList.add("kz-noanim");for(var sq in pos){var pc=pos[sq];pc.el=makePiece(pc);board.appendChild(pc.el);place(pc.el,sq);}hideHL();void board.offsetWidth;board.classList.remove("kz-noanim");}
function doMove(i,animate){var from=UCI[i].slice(0,2),to=UCI[i].slice(2,4);var pc=pos[from];if(!pc){return;}var cap=pos[to];if(cap&&cap!==pc){if(animate){var ce=cap.el;ce.classList.add("kz-cap");setTimeout(function(){ce.remove();},420);}else{cap.el.remove();}}delete pos[from];pos[to]=pc;place(pc.el,to);showHL(from,to);}
function updateUI(){document.getElementById("kzPly").textContent=ply;document.getElementById("kzTurn").textContent=(ply>=UCI.length)?"End · looping…":(((ply%2)===0)?"Black":"White")+" to move";var chips=movesEl.children;for(var i=0;i<chips.length;i++){chips[i].classList.toggle("kz-on",i===ply-1);}if(ply-1>=0&&chips[ply-1]){movesEl.scrollTop=chips[ply-1].offsetTop-64;}document.getElementById("kzPlay").innerHTML=playing?"&#10074;&#10074;":"&#9658;";}
function step(){if(ply<UCI.length){doMove(ply,true);ply++;updateUI();}}
function jumpTo(n){rebuild();board.classList.add("kz-noanim");for(var i=0;i<n;i++){doMove(i,false);}ply=n;void board.offsetWidth;board.classList.remove("kz-noanim");updateUI();}
function clearTimer(){if(timer){clearTimeout(timer);timer=null;}}
function schedule(){clearTimer();if(playing){timer=setTimeout(tick,SPEEDS[spi]);}}
function tick(){if(!playing){return;}if(ply>=UCI.length){timer=setTimeout(function(){jumpTo(0);schedule();},1500);return;}step();schedule();}
function setPlaying(v){playing=v;updateUI();if(playing){schedule();}else{clearTimer();}}
for(var m=0;m<SAN.length;m++){(function(idx){var c=document.createElement("button");c.className="kz-chip "+(((idx%2)===0)?"kz-chip--b":"kz-chip--w");c.textContent=SAN[idx];c.addEventListener("click",function(){setPlaying(false);jumpTo(idx+1);});movesEl.appendChild(c);})(m);}
document.getElementById("kzCtl").addEventListener("click",function(e){var b=e.target.closest?e.target.closest("button"):e.target;if(!b||!b.getAttribute){return;}var act=b.getAttribute("data-act");if(act==="play"){setPlaying(!playing);}else if(act==="next"){setPlaying(false);step();}else if(act==="prev"){setPlaying(false);jumpTo(Math.max(0,ply-1));}else if(act==="restart"){jumpTo(0);setPlaying(true);}else if(act==="flip"){flip=!flip;board.classList.add("kz-noanim");for(var sq in pos){place(pos[sq].el,sq);}relabel();if(curHL){showHL(curHL[0],curHL[1]);}void board.offsetWidth;board.classList.remove("kz-noanim");}else if(act==="speed"){spi=(spi+1)%SPEEDS.length;document.getElementById("kzSpeed").innerHTML=(spi===0?"1":spi===1?"&#189;":"2")+"&#215;";if(playing){schedule();}}});
function resize(){board.style.fontSize=(board.clientWidth/8*0.78)+"px";}
if(window.ResizeObserver){new ResizeObserver(resize).observe(board);}else{window.addEventListener("resize",resize);}
relabel();rebuild();resize();updateUI();schedule();
})();
</script>
</div>



<!-- My research interest includes neural machine translation and computer vision. I have published more than 100 papers at the top international AI conferences with total <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'>google scholar citations <strong><span id='total_cit'>260000+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>). -->


# 🔥 News
- 2026.06: Our paper **A Unified and Fast-Sampling Diffusion Bridge Framework via Stochastic Optimal Control** accepted by **IEEE TPAMI**!🎉🎉
- 2026.06: Our Team win the **Champion, Rapid U2200, FIDE World Team Rapid and Blitz Chess Championships 2026**!🎉🎉
- 2026.05: Our paper **Diffusion Bridge or Flow Matching? A Unifying Framework and Comparative Analysis** accepted by **ICML 2026** as a **Poster**!🎉🎉
- 2026.05: Our paper **Sample from What You See: Visuomotor Policy Learning via Diffusion Bridge with Observation-Embedded Stochastic Differential Equation** accepted by **ICML 2026** as a **Poster**!🎉🎉
- 2025.05: Our paper **UniDB: A Unified Diffusion Bridge Framework via Stochastic Optimal Control** accepted by **ICML 2025** as a **Spotlight**!🎉🎉
- 2025.04: Our paper **UniDB** won **Outstanding Paper Award** of ICLR 2025 DeLTa Workshop!🎉🎉
- 2025.04: Our paper **AffordDP: Generalizable Diffusion Policy with Transferable Affordance** accepted by **CVPR 2025**!🎉🎉

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TPAMI 2026</div><img src='images/unidb++.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**A Unified and Fast-Sampling Diffusion Bridge Framework via Stochastic Optimal Control, <span style="color:red;">IEEE TPAMI 2026.</span>**

 Mokai Pan\#, **Kaizhen Zhu\#**, Yuexin Ma, Yanwei Fu, Jingyi Yu, Jingya Wang, Ye Shi\*

[[**paper**]](https://arxiv.org/abs/2505.21528)
[[**code**]](https://github.com/2769433owo/UniDB-plusplus)

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICML 2026 Poster</div><img src='images/DBP2.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Sample from What You See: Visuomotor Policy Learning via Diffusion Bridge with Observation-Embedded Stochastic Differential Equation, <span style="color:red;">ICML 2026 Poster.</span>**

Zhaoyang Liu, Mokai Pan, Zhongyi Wang, **Kaizhen Zhu**, Haotao Lu, Jingya Wang, Ye Shi\*

[[**paper**]](https://arxiv.org/pdf/2512.07212)

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICML 2026 Poster</div><img src='images/DBFM2.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Diffusion Bridge or Flow Matching? A Unifying Framework and Comparative Analysis, <span style="color:red;">ICML 2026 Poster.</span>**

**Kaizhen Zhu\#**, Mokai Pan\#, Zhechuan Yu, Jingyi Yu, Jingya Wang, Ye Shi\*

[[**paper**]](https://arxiv.org/pdf/2509.24531v1)
[[**code**]](https://anonymous.4open.science/r/DBFM-3E8E)

</div>
</div>



<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICML 2025 Spotlight</div><img src='images/UniDB.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**UniDB: A Unified Diffusion Bridge Framework via Stochastic Optimal Control, <span style="color:red;">ICML 2025 Spotlight.</span>**


**Kaizhen Zhu\#**, Mokai Pan\#, Yuexin Ma, Yanwei Fu, Jingyi Yu, Jingya Wang, Ye Shi\*

[[**paper**]](https://arxiv.org/abs/2502.05749)
[[**project**]](https://unidb-soc.github.io/UniDB_page)
[[**code**]](https://github.com/UniDB-SOC/UniDB)

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2025</div><img src='images/AffordDP.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**AffordDP: Generalizable Diffusion Policy with Transferable Affordance,	CVPR 2025.**

Shijie Wu\#, Yihang Zhu\#, Yunao Huang, **Kaizhen Zhu**, Jiayuan Gu, Jingyi Yu, Ye Shi\*, Jingya Wang\*

[[**paper**]](https://arxiv.org/abs/2412.03142)
[[**project**]](https://afforddp.github.io/)
[[**code**]](https://github.com/SshiJwu/AffordDP)

</div>
</div>


# 💻 Software

<div class="kz-soft">
<style>
.kz-soft{position:relative;margin:24px 0;padding:28px;border-radius:22px;background:linear-gradient(135deg,#1b2440 0%,#2a3a66 45%,#3b2c63 100%);box-shadow:0 18px 50px -12px rgba(20,24,60,.65),inset 0 1px 0 rgba(255,255,255,.08);color:#eef1fb;overflow:hidden;}
.kz-soft::before{content:"";position:absolute;inset:-45%;background:conic-gradient(from 0deg,transparent 0 70%,rgba(120,170,255,.30) 83%,transparent 93%);animation:kzsoftspin 13s linear infinite;z-index:0;pointer-events:none;}
@keyframes kzsoftspin{to{transform:rotate(360deg);}}
.kz-soft>*{position:relative;z-index:1;}
.kz-soft__title{font-size:30px;font-weight:800;letter-spacing:.3px;line-height:1.15;background:linear-gradient(90deg,#cfe0ff,#9db8ff 42%,#d9c6ff);-webkit-background-clip:text;background-clip:text;color:transparent;}
.kz-soft__sub{margin-top:7px;font-size:15px;color:#c4cdea;}
.kz-soft__chips{display:flex;flex-wrap:wrap;gap:9px;margin:16px 0 20px;}
.kz-chip{font-size:13px;padding:6px 13px;border-radius:999px;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.17);color:#e9eefc;transition:transform .2s ease,background .2s ease,border-color .2s ease;}
.kz-chip:hover{transform:translateY(-2px);background:rgba(140,180,255,.20);border-color:rgba(160,195,255,.5);}
.kz-soft__video{position:relative;border-radius:16px;overflow:hidden;line-height:0;box-shadow:0 16px 44px -10px rgba(0,0,0,.65),0 0 0 1px rgba(255,255,255,.10);}
.kz-soft__video video{display:block;width:100%;height:auto;border-radius:16px;}
@media(max-width:560px){.kz-soft{padding:18px;}.kz-soft__title{font-size:23px;}}
</style>
<div class="kz-soft__title">ChessPrep&nbsp;Lab</div>
<div class="kz-soft__sub">A local-first chess training workbench I built from scratch — opening prep, endgames, and engine sparring in one offline app.</div>
<div class="kz-soft__chips">
<span class="kz-chip">♟ Opening repertoire trainer</span>
<span class="kz-chip">🧩 300 complex endgames · 2650+ Elo</span>
<span class="kz-chip">🤖 Stockfish + Maia‑3 sparring</span>
<span class="kz-chip">🔌 Fully offline</span>
</div>
<div class="kz-soft__video">
<video controls preload="metadata" playsinline>
<source src="images/chessprep-lab-demo.mp4" type="video/mp4">
Your browser does not support the video tag. <a href="images/chessprep-lab-demo.mp4">Download the demo video</a>.
</video>
</div>
</div>


# 🎖 Honors and Awards
- *2026* Champion, Rapid U2200, FIDE World Team Rapid and Blitz Chess Championships 2026.
- *2023.6* First Prize, Zhejiang Provincial Mathematics Competition 2023.
- *2022.11* National First Prize, China Undergraduate Mathematical Contest in Modeling (CUMCM) 2022.
- *2022.8* Second Prize, National Undergraduate Electronic Design Contest (NUEDC) 2022.

# 📖 Educations
<div class='paper-box'><div class='paper-box-image'><div><img src='images/skd.png' alt="sym" width="95%"></div></div>
<div class='paper-box-text' markdown="1">

<span style="font-size:18px;">**ShanghaiTech University**</span>

*2024.09 - now*

School of Information Science and Technology

Major: M.S. in **Computer Science**

MoE Key Laboratory of Intelligent Perception and Human Machine Collaboration, VDI Center, YesAI Lab
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/hangdian.jpg' alt="sym" width="95%"></div></div>
<div class='paper-box-text' markdown="1">

<span style="font-size:18px;">**Hangzhou Dianzi University**</span>

*2020.09 - 2024.06*

School of Electronic Information

Major: B.E. in **Electronic Science and Technology**

</div>
</div>

<!-- # 💬 Invited Talks
- *2021.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/) -->

<!-- # 💻 Internships
- *2019.05 - 2020.02*, [Lorem](https://github.com/), China. -->
