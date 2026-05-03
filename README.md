<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Free Live Training — Chrisstars Mums Academy</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700;900&family=Plus+Jakarta+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300&display=swap" rel="stylesheet"/>
<style>
:root{
  --navy:#0a1628;--navy2:#0f1e38;--navy3:#162240;
  --blue:#1a56db;--blue2:#2563eb;--sky:#3b82f6;
  --gold:#f59e0b;--white:#ffffff;
  --soft:#94a3b8;--muted:#475569;
  --border:rgba(255,255,255,0.08);
  --green:#22c55e;
}
*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{
  background:var(--navy);color:var(--white);
  font-family:'Plus Jakarta Sans',sans-serif;
  font-size:16px;line-height:1.6;overflow-x:hidden;
}

/* TOP BAR */
.topbar{
  background:rgba(10,22,40,0.97);backdrop-filter:blur(12px);
  border-bottom:1px solid var(--border);
  padding:11px 24px;
  display:flex;align-items:center;justify-content:space-between;
  position:sticky;top:0;z-index:100;
}
.topbar-logo img{height:34px;width:auto;filter:brightness(1.05);}
.live-pill{
  display:flex;align-items:center;gap:7px;
  background:rgba(239,68,68,0.1);border:1px solid rgba(239,68,68,0.3);
  border-radius:30px;padding:5px 14px;
  font-size:0.7rem;font-weight:700;color:#ef4444;letter-spacing:0.1em;text-transform:uppercase;
}
.live-dot{
  width:7px;height:7px;background:#ef4444;border-radius:50%;
  animation:blink 1.4s infinite;
}
@keyframes blink{0%,100%{opacity:1;transform:scale(1);}50%{opacity:0.4;transform:scale(0.6);}}
.viewer-pill{
  display:flex;align-items:center;gap:6px;
  font-size:0.78rem;color:var(--soft);
  background:rgba(255,255,255,0.04);border:1px solid var(--border);
  border-radius:30px;padding:5px 14px;
}
.viewer-pill strong{color:var(--white);}

/* HERO */
.hero{
  position:relative;overflow:hidden;
  padding:50px 24px 42px;text-align:center;
  background:linear-gradient(160deg,#0d1e3a 0%,#0a1628 55%,#071220 100%);
  border-bottom:1px solid var(--border);
}
.glow1{
  position:absolute;top:-80px;left:50%;transform:translateX(-50%);
  width:700px;height:280px;
  background:radial-gradient(ellipse,rgba(26,86,219,0.16) 0%,transparent 70%);
  pointer-events:none;
}
.glow2{
  position:absolute;bottom:-60px;right:-80px;
  width:360px;height:280px;
  background:radial-gradient(ellipse,rgba(245,158,11,0.07) 0%,transparent 70%);
  pointer-events:none;
}
.hero-tag{
  display:inline-flex;align-items:center;gap:7px;
  background:rgba(26,86,219,0.1);border:1px solid rgba(26,86,219,0.28);
  color:#60a5fa;font-size:0.7rem;font-weight:600;
  letter-spacing:0.1em;text-transform:uppercase;
  padding:5px 14px;border-radius:30px;margin-bottom:20px;
}
.hero h1{
  font-family:'Playfair Display',serif;
  font-size:clamp(1.6rem,4.5vw,2.9rem);
  font-weight:900;line-height:1.18;letter-spacing:-0.02em;
  margin-bottom:14px;max-width:720px;
  margin-left:auto;margin-right:auto;
}
.hero h1 .ac{
  background:linear-gradient(90deg,#3b82f6,#93c5fd);
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;
}
.hero h1 .gd{
  background:linear-gradient(90deg,#f59e0b,#fcd34d);
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;
}
.hero-sub{
  color:var(--soft);font-size:0.92rem;font-weight:300;
  max-width:510px;margin:0 auto 22px;line-height:1.75;
}
.host-pill{
  display:inline-flex;align-items:center;gap:12px;
  background:rgba(255,255,255,0.04);border:1px solid var(--border);
  border-radius:50px;padding:8px 20px 8px 8px;margin-bottom:20px;
}
.host-pill img{
  width:42px;height:42px;border-radius:50%;object-fit:cover;
  border:2px solid var(--blue2);
}
.hp-name{font-size:0.82rem;font-weight:600;color:var(--white);text-align:left;}
.hp-title{font-size:0.7rem;color:var(--soft);}
.no-refresh{
  display:inline-flex;align-items:center;gap:6px;
  font-size:0.7rem;color:var(--muted);
  background:rgba(255,255,255,0.03);border:1px solid var(--border);
  padding:5px 14px;border-radius:6px;
}

/* MAIN GRID */
.main{
  max-width:1120px;margin:0 auto;
  padding:26px 16px 50px;
  display:grid;grid-template-columns:1fr 336px;gap:22px;
  align-items:start;position:relative;z-index:1;
}
@media(max-width:840px){
  .main{grid-template-columns:1fr;}
  .chat-col{order:2;}
}

/* VIDEO CARD */
.video-card{
  background:var(--navy2);border:1px solid var(--border);
  border-radius:16px;overflow:hidden;
  box-shadow:0 24px 64px rgba(0,0,0,0.5),0 0 0 1px rgba(26,86,219,0.08);
}
.video-ratio{position:relative;width:100%;padding-bottom:56.25%;background:#000;}
.video-ratio iframe{position:absolute;top:0;left:0;width:100%;height:100%;border:none;}
.v-overlay{
  position:absolute;inset:0;
  background:linear-gradient(160deg,rgba(10,22,40,0.93) 0%,rgba(10,22,40,0.84) 100%);
  display:flex;flex-direction:column;align-items:center;justify-content:center;
  cursor:pointer;z-index:2;transition:opacity 0.4s;
}
.v-overlay.gone{opacity:0;pointer-events:none;}
.play-ring{
  width:78px;height:78px;border-radius:50%;
  background:linear-gradient(135deg,var(--blue),var(--sky));
  display:flex;align-items:center;justify-content:center;
  margin-bottom:18px;
  box-shadow:0 0 40px rgba(37,99,235,0.5),0 0 80px rgba(37,99,235,0.2);
  animation:rpulse 2.5s ease infinite;transition:transform 0.2s;
}
.play-ring:hover{transform:scale(1.08);}
@keyframes rpulse{
  0%,100%{box-shadow:0 0 40px rgba(37,99,235,0.5),0 0 80px rgba(37,99,235,0.2);}
  50%{box-shadow:0 0 60px rgba(37,99,235,0.7),0 0 110px rgba(37,99,235,0.3);}
}
.ov-label{
  font-family:'Playfair Display',serif;
  font-size:1.05rem;font-weight:700;text-align:center;
}
.ov-label small{
  display:block;font-family:'Plus Jakarta Sans',sans-serif;
  font-size:0.76rem;font-weight:300;color:var(--soft);margin-top:3px;
}
.video-foot{
  display:flex;align-items:center;justify-content:space-between;
  padding:11px 18px;background:rgba(255,255,255,0.02);
  border-top:1px solid var(--border);
  font-size:0.76rem;color:var(--soft);flex-wrap:wrap;gap:8px;
}
.vf-l{display:flex;align-items:center;gap:6px;}
.vf-r{font-size:0.7rem;color:var(--muted);}

/* LOCK NOTICE */
.lock-note{
  margin-top:16px;
  background:rgba(26,86,219,0.05);
  border:1px solid rgba(26,86,219,0.15);
  border-radius:10px;padding:13px 18px;
  display:flex;align-items:center;gap:11px;
  font-size:0.8rem;color:var(--soft);
}
.lock-note .icon{font-size:1.2rem;flex-shrink:0;}

/* OFFER */
.offer-wrap{display:none;margin-top:20px;animation:riseUp 0.7s cubic-bezier(0.16,1,0.3,1) both;}
.offer-wrap.show{display:block;}
@keyframes riseUp{from{opacity:0;transform:translateY(40px);}to{opacity:1;transform:translateY(0);}}
.offer-card{
  background:linear-gradient(145deg,#0d1e3a 0%,#0a1628 100%);
  border:1px solid rgba(26,86,219,0.22);
  border-radius:16px;padding:30px 26px;
  position:relative;overflow:hidden;
}
.offer-card::before{
  content:'';position:absolute;top:-60px;right:-60px;
  width:240px;height:240px;
  background:radial-gradient(ellipse,rgba(26,86,219,0.1) 0%,transparent 70%);
  pointer-events:none;
}
.offer-card::after{
  content:'';position:absolute;bottom:-40px;left:-40px;
  width:200px;height:200px;
  background:radial-gradient(ellipse,rgba(245,158,11,0.06) 0%,transparent 70%);
  pointer-events:none;
}
.offer-eyebrow{
  display:inline-flex;align-items:center;gap:6px;
  background:rgba(34,197,94,0.1);border:1px solid rgba(34,197,94,0.28);
  color:#4ade80;font-size:0.7rem;font-weight:700;
  letter-spacing:0.1em;text-transform:uppercase;
  padding:4px 12px;border-radius:20px;margin-bottom:16px;
}
.offer-title{
  font-family:'Playfair Display',serif;
  font-size:1.4rem;font-weight:700;line-height:1.3;
  margin-bottom:6px;letter-spacing:-0.01em;
}
.offer-sub{font-size:0.83rem;color:var(--soft);margin-bottom:22px;font-weight:300;}
.offer-list{list-style:none;display:flex;flex-direction:column;gap:11px;margin-bottom:26px;}
.offer-list li{display:flex;align-items:flex-start;gap:10px;font-size:0.875rem;color:#cbd5e1;}
.chk{
  width:20px;height:20px;border-radius:50%;flex-shrink:0;margin-top:1px;
  background:rgba(34,197,94,0.12);border:1px solid rgba(34,197,94,0.3);
  display:flex;align-items:center;justify-content:center;
  font-size:0.62rem;color:#4ade80;
}
.price-row{display:flex;align-items:baseline;gap:12px;margin-bottom:6px;flex-wrap:wrap;}
.price{font-family:'Playfair Display',serif;font-size:2.2rem;font-weight:900;}
.price-old{font-size:1rem;color:var(--muted);text-decoration:line-through;}
.price-note{font-size:0.73rem;color:var(--muted);margin-bottom:22px;}
.cta-btn{
  display:block;width:100%;
  background:linear-gradient(135deg,#1a56db,#2563eb);
  color:#fff;font-family:'Plus Jakarta Sans',sans-serif;
  font-weight:700;font-size:1rem;text-align:center;
  padding:17px 24px;border-radius:12px;text-decoration:none;
  letter-spacing:0.01em;
  transition:transform 0.15s,box-shadow 0.15s;
  box-shadow:0 4px 24px rgba(26,86,219,0.4),inset 0 1px 0 rgba(255,255,255,0.14);
  border:none;cursor:pointer;position:relative;overflow:hidden;
}
.cta-btn::after{
  content:'';position:absolute;inset:0;
  background:linear-gradient(135deg,rgba(255,255,255,0.12) 0%,transparent 60%);
  pointer-events:none;
}
.cta-btn:hover{transform:translateY(-2px);box-shadow:0 8px 36px rgba(26,86,219,0.55);}
.trust-row{
  display:flex;justify-content:center;gap:12px;
  margin-top:13px;font-size:0.7rem;color:var(--muted);flex-wrap:wrap;
}
.cd-box{
  background:rgba(245,158,11,0.07);border:1px solid rgba(245,158,11,0.2);
  border-radius:10px;padding:13px 18px;
  margin-top:18px;text-align:center;
}
.cd-label{font-size:0.68rem;text-transform:uppercase;letter-spacing:0.1em;color:var(--gold);font-weight:600;margin-bottom:5px;}
.cd-num{font-family:'Playfair Display',serif;font-size:2rem;font-weight:900;color:var(--gold);letter-spacing:0.06em;}

/* CHAT */
.chat-card{
  background:var(--navy2);border:1px solid var(--border);
  border-radius:16px;overflow:hidden;
  display:flex;flex-direction:column;height:560px;
  position:sticky;top:64px;
  box-shadow:0 20px 50px rgba(0,0,0,0.4);
}
.chat-head{
  background:var(--navy3);border-bottom:1px solid var(--border);
  padding:13px 18px;display:flex;align-items:center;justify-content:space-between;
}
.ch-left{display:flex;align-items:center;gap:9px;font-weight:700;font-size:0.86rem;}
.g-dot{width:8px;height:8px;background:#22c55e;border-radius:50%;animation:blink 1.4s infinite;}
.ch-count{font-size:0.7rem;color:var(--muted);font-weight:400;}
.chat-body{
  flex:1;overflow-y:auto;padding:13px 13px 8px;
  display:flex;flex-direction:column;gap:11px;
  scrollbar-width:thin;scrollbar-color:#1a2540 transparent;
}
.chat-body::-webkit-scrollbar{width:3px;}
.chat-body::-webkit-scrollbar-thumb{background:#1a2540;border-radius:4px;}
.msg{opacity:0;transform:translateY(10px);animation:msgIn 0.45s ease forwards;}
@keyframes msgIn{to{opacity:1;transform:translateY(0);}}
.msg-name{font-size:0.7rem;font-weight:600;display:flex;align-items:center;gap:5px;margin-bottom:3px;}
.msg-bubble{
  font-size:0.79rem;color:#cbd5e1;line-height:1.55;
  background:var(--navy3);border:1px solid var(--border);
  border-radius:2px 10px 10px 10px;padding:8px 12px;max-width:96%;
}
.chat-foot{border-top:1px solid var(--border);padding:10px 12px;background:var(--navy3);}
.chat-foot .r1{display:flex;gap:6px;margin-bottom:6px;}
.chat-foot input{
  flex:1;background:var(--navy2);border:1px solid var(--border);
  border-radius:8px;padding:8px 11px;
  font-family:'Plus Jakarta Sans',sans-serif;font-size:0.76rem;
  color:var(--white);outline:none;transition:border-color 0.2s;
}
.chat-foot input:focus{border-color:rgba(26,86,219,0.5);}
.chat-foot input::placeholder{color:var(--muted);}
.chat-foot .r2{display:flex;gap:6px;}
.send-btn{
  background:var(--blue2);border:none;border-radius:8px;
  padding:8px 13px;color:#fff;font-size:0.76rem;font-weight:600;
  cursor:pointer;transition:background 0.2s;white-space:nowrap;
}
.send-btn:hover{background:var(--blue);}

/* STICKY */
.sticky{
  position:fixed;bottom:0;left:0;right:0;
  background:rgba(10,22,40,0.97);backdrop-filter:blur(14px);
  border-top:1px solid rgba(26,86,219,0.28);
  padding:12px 20px;
  display:none;align-items:center;justify-content:space-between;
  z-index:200;gap:12px;flex-wrap:wrap;
}
.sticky.on{display:flex;}
.st-text{font-size:0.86rem;font-weight:700;}
.st-text span{display:block;font-weight:300;font-size:0.73rem;color:var(--soft);}
.st-cd{font-family:'Playfair Display',serif;font-size:1.1rem;font-weight:900;color:var(--gold);}
.st-btn{
  background:linear-gradient(135deg,#1a56db,#2563eb);color:#fff;
  font-weight:700;font-size:0.8rem;
  padding:11px 20px;border-radius:8px;text-decoration:none;white-space:nowrap;
  box-shadow:0 4px 20px rgba(26,86,219,0.4);transition:transform 0.15s;
}
.st-btn:hover{transform:translateY(-1px);}

/* FOOTER */
footer{
  border-top:1px solid var(--border);text-align:center;
  padding:28px 20px;font-size:0.73rem;color:var(--muted);
  position:relative;z-index:1;
}
footer img{height:26px;width:auto;display:block;margin:0 auto 10px;opacity:0.65;}
</style>
</head>
<body>

<!-- TOP BAR -->
<div class="topbar">
  <div class="topbar-logo">
    <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAgICAgJCAkKCgkNDgwODRMREBARExwUFhQWFBwrGx8bGx8bKyYuJSMlLiZENS8vNUROQj5CTl9VVV93cXecnNEBCAgICAkICQoKCQ0ODA4NExEQEBETHBQWFBYUHCsbHxsbHxsrJi4lIyUuJkQ1Ly81RE5CPkJOX1VVX3dxd5yc0f/CABEICAAKAAMBIgACEQEDEQH/xAAxAAEAAwEBAQAAAAAAAAAAAAAABAUGAwIBAQEBAQEBAQAAAAAAAAAAAAAAAgEDBAX/2gAMAwEAAhADEAAAAr8AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
