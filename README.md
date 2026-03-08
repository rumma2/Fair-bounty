<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FairBounty — Full Infographic</title>
<link href="https://fonts.googleapis.com/css2?family=Righteous&family=Nunito:wght@300;400;600;800;900&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --sky:#5BC8F5;--sky2:#2FAEE0;--sky3:#A8E4FF;--skydeep:#0D4F78;
  --white:#FFFFFF;--cream:#F0FAFF;--ink:#0D2137;--ink2:#1B3F6A;
  --gold:#FFD166;--coral:#FF7B72;--mint:#06D6A0;--purple:#A78BFA;
  --lavender:#EDE9FE;--paleblue:#D6F0FB;
}
body{
  background:#0D2137;
  font-family:'Nunito',sans-serif;
  display:flex;align-items:flex-start;justify-content:center;
  min-height:100vh;padding:28px 16px;
}
.poster{
  width:100%;max-width:920px;border-radius:32px;overflow:hidden;
  box-shadow:0 48px 140px rgba(0,0,0,.75),0 0 0 1px rgba(91,200,245,.18);
}

/* ══ HERO ══ */
.hero{
  position:relative;
  background:linear-gradient(155deg,#5BC8F5 0%,#2FAEE0 35%,#1587BB 65%,#0D4F78 100%);
  padding:52px 52px 70px;overflow:hidden;min-height:340px;
  display:flex;flex-direction:column;justify-content:flex-end;
}
.hero::before{
  content:'';position:absolute;inset:0;
  background:
    radial-gradient(ellipse 65% 45% at 78% 18%,rgba(255,255,255,.28) 0%,transparent 60%),
    radial-gradient(ellipse 80% 50% at 50% -8%,rgba(255,255,255,.16) 0%,transparent 68%);
}
.hero-art{position:absolute;top:0;right:0;width:56%;height:100%;z-index:1;}
.hero-content{position:relative;z-index:2;max-width:440px;}
.launch-badge{
  display:inline-flex;align-items:center;gap:8px;
  background:rgba(255,209,102,.18);backdrop-filter:blur(10px);
  border:1.5px solid rgba(255,209,102,.5);border-radius:999px;
  padding:7px 18px;margin-bottom:18px;
  font-size:11px;font-weight:800;color:var(--gold);letter-spacing:1.5px;text-transform:uppercase;
}
.launch-dot{width:7px;height:7px;border-radius:50%;background:var(--gold);animation:blink 1.6s infinite;}
@keyframes blink{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.3;transform:scale(.7)}}
.hero h1{
  font-family:'Righteous',sans-serif;
  font-size:clamp(46px,7vw,74px);line-height:.92;color:white;
  text-shadow:0 4px 28px rgba(0,0,0,.22);margin-bottom:14px;
}
.hero h1 em{
  font-style:normal;
  background:linear-gradient(90deg,#FFD166 0%,#fff 100%);
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;
}
.hero-sub{font-size:15px;font-weight:400;line-height:1.65;color:rgba(255,255,255,.86);max-width:380px;margin-bottom:22px;}
.hero-pills{display:flex;gap:8px;flex-wrap:wrap;}
.hero-pill{
  font-family:'Space Mono',monospace;font-size:9px;letter-spacing:1.5px;text-transform:uppercase;
  padding:5px 12px;border-radius:999px;
  background:rgba(255,255,255,.14);border:1px solid rgba(255,255,255,.3);color:white;
}

/* wave */
.wave-div{background:linear-gradient(155deg,#5BC8F5 0%,#0D4F78 100%);line-height:0;margin-top:-2px;}
.wave-div svg{display:block;width:100%;}

/* ══ BODY ══ */
.body{background:var(--cream);padding:52px 48px;display:flex;flex-direction:column;gap:52px;}

/* section header */
.sh{display:flex;align-items:center;gap:12px;margin-bottom:26px;}
.sh-num{font-family:'Space Mono',monospace;font-size:10px;font-weight:700;color:var(--sky2);letter-spacing:2px;}
.sh-title{font-family:'Righteous',sans-serif;font-size:21px;color:var(--ink);}
.sh-line{flex:1;height:2px;border-radius:2px;background:linear-gradient(90deg,var(--sky),transparent);}

/* ══ WHAT IS FAIRBOUNTY ══ */
.what-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;}
.what-left{
  background:linear-gradient(155deg,var(--ink2),var(--ink));
  border-radius:22px;padding:32px 28px;
  display:flex;flex-direction:column;gap:18px;
  position:relative;overflow:hidden;
}
.what-left::after{
  content:'';position:absolute;width:220px;height:220px;border-radius:50%;
  background:radial-gradient(circle,rgba(91,200,245,.12) 0%,transparent 70%);
  top:-60px;right:-60px;pointer-events:none;
}
.what-title{font-family:'Righteous',sans-serif;font-size:22px;color:var(--sky3);line-height:1.2;}
.what-desc{font-size:13px;color:rgba(255,255,255,.7);line-height:1.65;}
.what-bullets{display:flex;flex-direction:column;gap:10px;}
.wb{display:flex;align-items:flex-start;gap:12px;}
.wb-icon{
  width:34px;height:34px;border-radius:10px;flex-shrink:0;
  display:flex;align-items:center;justify-content:center;font-size:17px;
  background:rgba(91,200,245,.15);border:1px solid rgba(91,200,245,.25);
}
.wb-text h4{font-size:13px;font-weight:800;color:white;margin-bottom:2px;}
.wb-text p{font-size:12px;font-weight:400;color:rgba(255,255,255,.5);line-height:1.4;}

.what-right{display:flex;flex-direction:column;gap:14px;}
.info-card{
  border-radius:18px;padding:20px 20px;
  display:flex;align-items:center;gap:14px;
  box-shadow:0 4px 18px rgba(13,33,55,.09);
  transition:transform .25s;
}
.info-card:hover{transform:translateX(5px);}
.info-card.ic1{background:linear-gradient(135deg,#EFF9FF,#D6F0FB);border-left:4px solid var(--sky);}
.info-card.ic2{background:linear-gradient(135deg,#FFFBEB,#FEF3C7);border-left:4px solid var(--gold);}
.info-card.ic3{background:linear-gradient(135deg,#ECFDF5,#D1FAE5);border-left:4px solid var(--mint);}
.info-card.ic4{background:linear-gradient(135deg,#F5F3FF,#EDE9FE);border-left:4px solid var(--purple);}
.ic-bubble{
  width:46px;height:46px;border-radius:14px;flex-shrink:0;
  display:flex;align-items:center;justify-content:center;font-size:22px;
}
.ic1 .ic-bubble{background:rgba(91,200,245,.2);}
.ic2 .ic-bubble{background:rgba(255,209,102,.2);}
.ic3 .ic-bubble{background:rgba(6,214,160,.2);}
.ic4 .ic-bubble{background:rgba(167,139,250,.2);}
.ic-text h4{font-size:13px;font-weight:800;color:var(--ink);margin-bottom:3px;}
.ic-text p{font-size:12px;color:#5a7a96;line-height:1.4;}

/* ══ HOW IT WORKS ══ */
.steps{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;}
.step-card{border-radius:20px;overflow:hidden;box-shadow:0 6px 28px rgba(13,33,55,.1);transition:transform .3s,box-shadow .3s;}
.step-card:hover{transform:translateY(-6px);box-shadow:0 18px 46px rgba(13,33,55,.17);}
.step-art{height:120px;position:relative;overflow:hidden;}
.step-art svg{position:absolute;inset:0;width:100%;height:100%;}
.step-body{background:white;padding:16px 18px 20px;}
.step-lbl{font-family:'Space Mono',monospace;font-size:9px;letter-spacing:2px;text-transform:uppercase;margin-bottom:5px;}
.step-body h3{font-size:15px;font-weight:800;color:var(--ink);margin-bottom:5px;}
.step-body p{font-size:12px;color:#5a7a96;line-height:1.55;}
.sc1 .step-lbl{color:var(--sky2);}
.sc2 .step-lbl{color:var(--purple);}
.sc3 .step-lbl{color:var(--mint);}

/* ══ JOURNEY FLOW ══ */
.journey{background:white;border-radius:24px;padding:32px 30px;box-shadow:0 4px 20px rgba(13,33,55,.07);}
.flow-row{display:flex;align-items:center;justify-content:space-between;gap:4px;flex-wrap:wrap;}
.fn{display:flex;flex-direction:column;align-items:center;gap:8px;flex:1;min-width:80px;}
.fb{
  width:68px;height:68px;border-radius:50%;
  display:flex;align-items:center;justify-content:center;font-size:28px;
  transition:transform .3s;
}
.fb:hover{transform:scale(1.12);}
.fb.b1{background:linear-gradient(135deg,#A8E4FF,#5BC8F5);box-shadow:0 6px 22px rgba(91,200,245,.4);}
.fb.b2{background:linear-gradient(135deg,#C4B5FD,#A78BFA);box-shadow:0 6px 22px rgba(167,139,250,.4);}
.fb.b3{background:linear-gradient(135deg,#FDE68A,#FFD166);box-shadow:0 6px 22px rgba(255,209,102,.4);}
.fb.b4{background:linear-gradient(135deg,#6EE7B7,#06D6A0);box-shadow:0 6px 22px rgba(6,214,160,.4);}
.fb.b5{background:linear-gradient(135deg,#FCA5A5,#FF7B72);box-shadow:0 6px 22px rgba(255,123,114,.4);}
.fn span{font-size:12px;font-weight:800;color:var(--ink);text-align:center;}
.fn small{font-size:10px;color:#8aacbf;text-align:center;line-height:1.3;}
.fa{flex-shrink:0;font-size:20px;color:#c5dcea;animation:hop 1.8s ease-in-out infinite;}
@keyframes hop{0%,100%{transform:translateX(0)}50%{transform:translateX(5px)}}

/* ══ TOKEN LAUNCH ══ */
.token-section{display:grid;grid-template-columns:1.1fr 1fr;gap:20px;}
.token-hero-card{
  border-radius:24px;overflow:hidden;
  background:linear-gradient(155deg,#1B3F6A,#0D2137);
  padding:36px 30px;
  display:flex;flex-direction:column;gap:20px;
  position:relative;overflow:hidden;
  box-shadow:0 8px 32px rgba(13,33,55,.18);
}
.token-hero-card::before{
  content:'$BOUNTY';
  position:absolute;bottom:-14px;right:-10px;
  font-family:'Righteous',sans-serif;font-size:68px;
  color:rgba(255,209,102,.07);letter-spacing:-2px;pointer-events:none;
}
.token-hero-card::after{
  content:'';position:absolute;width:200px;height:200px;border-radius:50%;
  background:radial-gradient(circle,rgba(255,209,102,.12) 0%,transparent 70%);
  top:-50px;right:-50px;pointer-events:none;
}
.coin-wrap{display:flex;align-items:center;gap:18px;position:relative;z-index:1;}
.coin{
  width:76px;height:76px;border-radius:50%;flex-shrink:0;
  background:conic-gradient(from 180deg,#FFD166,#FFA500,#FFD166,#FFEC99,#FFD166);
  display:flex;align-items:center;justify-content:center;
  animation:coinPulse 3s ease-in-out infinite;
}
@keyframes coinPulse{
  0%,100%{box-shadow:0 0 0 6px rgba(255,209,102,.15),0 0 36px rgba(255,209,102,.3);}
  50%{box-shadow:0 0 0 12px rgba(255,209,102,.08),0 0 60px rgba(255,209,102,.55);}
}
.coin-inner{
  width:58px;height:58px;border-radius:50%;
  background:linear-gradient(135deg,#FFD166,#CC8800);
  display:flex;align-items:center;justify-content:center;
  font-family:'Space Mono',monospace;font-size:9px;font-weight:700;
  color:#7A4F00;text-align:center;line-height:1.3;
}
.coin-info{}
.coin-info h3{font-family:'Righteous',sans-serif;font-size:22px;color:var(--gold);margin-bottom:4px;}
.coin-info p{font-size:12px;color:rgba(255,255,255,.55);line-height:1.45;}

.launch-banner{
  background:rgba(255,209,102,.1);border:1px solid rgba(255,209,102,.3);
  border-radius:14px;padding:14px 16px;
  position:relative;z-index:1;
}
.launch-banner .lb-title{
  font-family:'Space Mono',monospace;font-size:10px;letter-spacing:2px;text-transform:uppercase;
  color:var(--gold);margin-bottom:8px;display:flex;align-items:center;gap:7px;
}
.lb-dot{width:6px;height:6px;border-radius:50%;background:var(--gold);animation:blink 1.5s infinite;}
.launch-banner p{font-size:12px;color:rgba(255,255,255,.65);line-height:1.5;}

.token-uses-col{display:flex;flex-direction:column;gap:12px;justify-content:center;}
.use-card{
  border-radius:16px;padding:16px 18px;
  display:flex;align-items:center;gap:14px;
  transition:transform .25s;
  box-shadow:0 3px 14px rgba(13,33,55,.08);
}
.use-card:hover{transform:translateX(4px);}
.use-card.u1{background:linear-gradient(135deg,#EFF9FF,#D6F0FB);border-left:4px solid var(--sky);}
.use-card.u2{background:linear-gradient(135deg,#FFFBEB,#FEF3C7);border-left:4px solid var(--gold);}
.use-card.u3{background:linear-gradient(135deg,#ECFDF5,#D1FAE5);border-left:4px solid var(--mint);}
.ui-wrap{width:44px;height:44px;border-radius:12px;flex-shrink:0;display:flex;align-items:center;justify-content:center;font-size:22px;}
.u1 .ui-wrap{background:rgba(91,200,245,.18);}
.u2 .ui-wrap{background:rgba(255,209,102,.18);}
.u3 .ui-wrap{background:rgba(6,214,160,.18);}
.use-card h4{font-size:13px;font-weight:800;color:var(--ink);margin-bottom:3px;}
.use-card p{font-size:11px;color:#6b8da6;line-height:1.4;}

/* ══ TOKEN FLOW DIAGRAM ══ */
.token-flow{background:white;border-radius:22px;padding:28px 30px;box-shadow:0 4px 18px rgba(13,33,55,.07);}
.tflow-row{display:flex;align-items:stretch;gap:0;margin-top:16px;}
.tflow-node{
  flex:1;border-radius:16px;padding:18px 14px;text-align:center;
  display:flex;flex-direction:column;align-items:center;gap:8px;
  transition:transform .3s;
}
.tflow-node:hover{transform:scale(1.04);}
.tflow-node.tn1{background:linear-gradient(155deg,#EFF9FF,#D6F0FB);}
.tflow-node.tn2{background:linear-gradient(155deg,#FFFBEB,#FEF3C7);}
.tflow-node.tn3{background:linear-gradient(155deg,#F5F3FF,#EDE9FE);}
.tflow-node.tn4{background:linear-gradient(155deg,#ECFDF5,#D1FAE5);}
.tflow-icon{font-size:30px;filter:drop-shadow(0 3px 8px rgba(0,0,0,.1));}
.tflow-lbl{font-size:12px;font-weight:800;color:var(--ink);}
.tflow-sub{font-size:10px;color:#7a9cb0;line-height:1.35;text-align:center;}
.tflow-arr{
  flex-shrink:0;width:28px;display:flex;align-items:center;justify-content:center;
  color:var(--sky);font-size:18px;opacity:.6;
  animation:hop 2s ease-in-out infinite;
}

/* ══ REPUTATION ══ */
.rep-row{display:grid;grid-template-columns:repeat(4,1fr);gap:14px;}
.tier-card{border-radius:20px;overflow:hidden;box-shadow:0 4px 18px rgba(13,33,55,.09);transition:transform .3s;}
.tier-card:hover{transform:translateY(-5px);}
.tier-top{height:88px;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:5px;}
.tier-gem{font-size:32px;filter:drop-shadow(0 3px 8px rgba(0,0,0,.2));}
.tier-top .tlbl{font-family:'Space Mono',monospace;font-size:9px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:white;}
.tier-card.bronze .tier-top{background:linear-gradient(135deg,#C97B2F,#8B5A1A);}
.tier-card.silver .tier-top{background:linear-gradient(135deg,#9BA3B0,#6B7785);}
.tier-card.gold   .tier-top{background:linear-gradient(135deg,#FFD166,#C89000);}
.tier-card.diamond .tier-top{background:linear-gradient(135deg,#5BC8F5,#1587BB);}
.tier-body{background:white;padding:13px;text-align:center;}
.tier-body h4{font-size:13px;font-weight:800;color:var(--ink);margin-bottom:3px;}
.tier-body p{font-size:11px;color:#7a9cb0;line-height:1.35;}

/* ══ SUBMISSION REQUIREMENTS ══ */
.sub-req{
  background:linear-gradient(155deg,var(--ink2),var(--ink));
  border-radius:24px;padding:36px 36px;
  position:relative;overflow:hidden;
}
.sub-req::before{
  content:'';position:absolute;width:300px;height:300px;border-radius:50%;
  background:radial-gradient(circle,rgba(91,200,245,.08) 0%,transparent 70%);
  top:-80px;right:-80px;pointer-events:none;
}
.sub-req::after{
  content:'';position:absolute;width:200px;height:200px;border-radius:50%;
  background:radial-gradient(circle,rgba(255,209,102,.07) 0%,transparent 70%);
  bottom:-50px;left:-30px;pointer-events:none;
}
.sub-inner{position:relative;z-index:1;}
.sub-cols{display:grid;grid-template-columns:1fr 1fr;gap:24px;margin-top:4px;}
.sub-col h4{
  font-family:'Space Mono',monospace;font-size:10px;letter-spacing:2px;text-transform:uppercase;
  color:var(--sky);margin-bottom:14px;
  display:flex;align-items:center;gap:8px;
}
.sub-col h4.bonus{color:var(--gold);}
.sub-col h4::after{content:'';flex:1;height:1px;background:rgba(91,200,245,.2);}
.sub-col h4.bonus::after{background:rgba(255,209,102,.2);}
.sub-items{display:flex;flex-direction:column;gap:10px;}
.si{display:flex;align-items:flex-start;gap:10px;}
.si-dot{
  width:22px;height:22px;border-radius:7px;flex-shrink:0;margin-top:1px;
  display:flex;align-items:center;justify-content:center;font-size:11px;
  background:rgba(91,200,245,.15);
}
.si-dot.bonus-dot{background:rgba(255,209,102,.15);}
.si p{font-size:13px;color:rgba(255,255,255,.72);line-height:1.5;}
.si p strong{color:white;font-weight:800;}

/* ══ SOCIAL BANNER ══ */
.social-banner{
  background:linear-gradient(135deg,rgba(91,200,245,.12),rgba(255,209,102,.08));
  border:1px solid rgba(91,200,245,.2);
  border-radius:18px;padding:22px 24px;
  display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:14px;
}
.sb-left{}
.sb-left h4{font-family:'Righteous',sans-serif;font-size:17px;color:var(--ink);margin-bottom:5px;}
.sb-left p{font-size:13px;color:#5a7a96;}
.sb-platforms{display:flex;gap:10px;flex-wrap:wrap;}
.sp{
  display:flex;align-items:center;gap:7px;
  background:white;border-radius:12px;padding:9px 16px;
  font-size:12px;font-weight:800;color:var(--ink);
  box-shadow:0 2px 10px rgba(13,33,55,.08);
  transition:transform .2s;
}
.sp:hover{transform:translateY(-2px);}

/* ══ FOOTER ══ */
.footer{
  background:linear-gradient(135deg,#0D2137,#1B3F6A);
  padding:26px 52px;
  display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:14px;
}
.flogo{font-family:'Righteous',sans-serif;font-size:20px;color:white;display:flex;align-items:center;gap:9px;}
.flogo span{color:var(--sky3);}
.flogo-dot{width:7px;height:7px;border-radius:50%;background:var(--gold);}
.ftags{display:flex;gap:7px;flex-wrap:wrap;}
.ftag{
  font-family:'Space Mono',monospace;font-size:9px;letter-spacing:1.5px;text-transform:uppercase;
  padding:5px 11px;border-radius:999px;
  border:1px solid rgba(91,200,245,.28);color:var(--sky3);background:rgba(91,200,245,.07);
}
.fcta{font-size:12px;color:rgba(255,255,255,.45);font-style:italic;}

/* ══ RESPONSIVE ══ */
@media(max-width:680px){
  .hero{padding:40px 26px 56px;}
  .body{padding:36px 22px;gap:36px;}
  .what-grid{grid-template-columns:1fr;}
  .steps{grid-template-columns:1fr;}
  .token-section{grid-template-columns:1fr;}
  .rep-row{grid-template-columns:repeat(2,1fr);}
  .sub-cols{grid-template-columns:1fr;}
  .fa{display:none;}
  .footer{padding:22px 26px;flex-direction:column;align-items:flex-start;}
  .tflow-arr{display:none;}
  .tflow-row{flex-wrap:wrap;}
}
</style>
</head>
<body>
<div class="poster">

<!-- ══ HERO ══ -->
<div class="hero">
  <svg class="hero-art" viewBox="0 0 500 340" fill="none" xmlns="http://www.w3.org/2000/svg">
    <!-- Sky glow -->
    <circle cx="360" cy="82" r="100" fill="rgba(255,255,255,0.06)"/>
    <circle cx="360" cy="82" r="62"  fill="rgba(255,255,255,0.09)"/>
    <circle cx="360" cy="82" r="34"  fill="rgba(255,255,255,0.15)"/>
    <!-- Clouds -->
    <ellipse cx="278" cy="58" rx="74" ry="28" fill="rgba(255,255,255,0.21)"/>
    <ellipse cx="312" cy="44" rx="48" ry="23" fill="rgba(255,255,255,0.21)"/>
    <ellipse cx="244" cy="50" rx="40" ry="19" fill="rgba(255,255,255,0.16)"/>
    <ellipse cx="430" cy="130" rx="54" ry="21" fill="rgba(255,255,255,0.13)"/>
    <ellipse cx="456" cy="119" rx="34" ry="17" fill="rgba(255,255,255,0.13)"/>
    <!-- Stars -->
    <circle cx="158" cy="26" r="3"   fill="rgba(255,255,255,0.75)"/>
    <circle cx="404" cy="42" r="2.5" fill="rgba(255,255,255,0.65)"/>
    <circle cx="194" cy="110" r="2"  fill="rgba(255,255,255,0.5)"/>
    <circle cx="462" cy="175" r="2"  fill="rgba(255,255,255,0.4)"/>
    <!-- Artist figure -->
    <g transform="translate(322,152)">
      <ellipse cx="0" cy="82" rx="29" ry="41" fill="#1A4C72"/>
      <circle cx="0" cy="28" r="27" fill="#F4C490"/>
      <ellipse cx="0" cy="14" rx="27" ry="17" fill="#3D2B1F"/>
      <ellipse cx="0"  cy="4" rx="23" ry="9"  fill="#5BC8F5"/>
      <circle cx="0"   cy="0" r="5.5"         fill="#2FAEE0"/>
      <circle cx="-10" cy="29" r="3.5" fill="white"/>
      <circle cx="10"  cy="29" r="3.5" fill="white"/>
      <circle cx="-9"  cy="29" r="1.8" fill="#222"/>
      <circle cx="11"  cy="29" r="1.8" fill="#222"/>
      <path d="M-9 37 Q0 44 9 37" stroke="#C47A3A" stroke-width="1.5" fill="none" stroke-linecap="round"/>
      <rect x="-48" y="55" width="22" height="10" rx="5" fill="#1A4C72" transform="rotate(25,-48,55)"/>
      <rect x="28"  y="55" width="22" height="10" rx="5" fill="#1A4C72" transform="rotate(-20,28,55)"/>
      <circle cx="-38" cy="73" r="8.5" fill="#F4C490"/>
      <ellipse cx="47" cy="71" rx="17" ry="13" fill="#E8D5B0"/>
      <circle cx="41" cy="67" r="4.5" fill="#FF7B72"/>
      <circle cx="51" cy="63" r="3.5" fill="#5BC8F5"/>
      <circle cx="55" cy="73" r="3.5" fill="#06D6A0"/>
      <circle cx="44" cy="75" r="3.5" fill="#FFD166"/>
      <line x1="-36" y1="73" x2="-11" y2="50" stroke="#8B6341" stroke-width="2.5"/>
      <ellipse cx="-10" cy="49" rx="5.5" ry="3" fill="#5BC8F5" transform="rotate(-35,-10,49)"/>
    </g>
    <!-- Artwork canvas on easel -->
    <g transform="translate(146,126)">
      <rect width="116" height="92" rx="6" fill="white" opacity="0.93"/>
      <rect x="8" y="8" width="100" height="76" rx="4" fill