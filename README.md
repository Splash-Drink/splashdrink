<!DOCTYPE html>
<html lang="hu">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Flash Drink</title>
<style>
* { margin:0; padding:0; box-sizing:border-box; font-family: Arial, sans-serif; }
body { background:black; color:white; overflow-x:hidden; }
body::before { content:""; position:fixed; inset:-50%; background: radial-gradient(circle, rgba(234,255,0,0.15), transparent 40%); animation: explosion 6s infinite ease-in-out; z-index:-2; }
@keyframes explosion { 0% { transform: scale(0.8); opacity:0.3; } 50% { transform: scale(1.2); opacity:0.6; } 100% { transform: scale(0.8); opacity:0.3; } }
.particles { position:fixed; inset:0; z-index:-1; }
.particle { position:absolute; width:6px; height:6px; background:#eaff00; border-radius:50%; opacity:0.6; animation: float 10s linear infinite; box-shadow:0 0 15px #eaff00; }
@keyframes float { from { transform: translateY(100vh) scale(0); } to { transform: translateY(-10vh) scale(1); } }
.hero { min-height:100vh; display:flex; justify-content:center; align-items:center; text-align:center; padding:40px 20px; }
h1 { font-size:clamp(40px,8vw,100px); font-weight:900; letter-spacing:3px; animation: glowPulse 2.5s infinite ease-in-out; }
.neon { color:#eaff00; text-shadow:0 0 10px #eaff00, 0 0 25px #eaff00, 0 0 50px #eaff00; }
@keyframes glowPulse { 0% { text-shadow:0 0 10px #eaff00; } 50% { text-shadow:0 0 40px #eaff00; } 100% { text-shadow:0 0 10px #eaff00; } }
.subtitle { margin-top:20px; font-size:18px; color:rgba(255,255,255,0.7); animation: fadeInUp 1s ease forwards; }
.btn { margin-top:35px; padding:16px 34px; border-radius:40px; border:none; background:#eaff00; color:black; font-weight:bold; font-size:16px; cursor:pointer; box-shadow:0 0 35px rgba(234,255,0,0.6); transition:0.25s; animation: btnGlow 2s infinite ease-in-out; }
.btn:hover { transform:scale(1.1); }
@keyframes btnGlow { 0% { box-shadow:0 0 20px rgba(234,255,0,0.4); } 50% { box-shadow:0 0 50px rgba(234,255,0,0.9); } 100% { box-shadow:0 0 20px rgba(234,255,0,0.4); } }
.section { padding:80px 20px; text-align:center; animation: fadeInUp 1s ease forwards; }
@keyframes fadeInUp { from { opacity:0; transform:translateY(30px); } to { opacity:1; transform:translateY(0); } }
.cards { display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:20px; margin-top:40px; max-width:900px; margin-inline:auto; }
.card { background: rgba(255,255,255,0.05); border-radius:20px; padding:25px; border:1px solid rgba(255,255,0,0.2); transition:0.3s; }
.card:hover { transform:translateY(-10px) scale(1.03); box-shadow:0 0 30px rgba(234,255,0,0.25); }
.card h3 { margin-bottom:10px; color:#eaff00; }
footer { text-align:center; padding:40px 20px; color:rgba(255,255,255,0.4); }
.shop { margin-top:60px; text-align:center; }
.shop button { margin:10px; padding:14px 28px; border-radius:30px; border:none; background:#eaff00; color:black; font-weight:bold; cursor:pointer; box-shadow:0 0 25px rgba(234,255,0,0.4); transition:0.2s; }
.shop button:hover { transform:scale(1.05); }
</style>
</head>
<body>
<div class="particles">
<div class="particle" style="left:10%; animation-delay:0s;"></div>
<div class="particle" style="left:30%; animation-delay:2s;"></div>
<div class="particle" style="left:50%; animation-delay:4s;"></div>
<div class="particle" style="left:70%; animation-delay:1s;"></div>
<div class="particle" style="left:90%; animation-delay:3s;"></div>
</div>

<section class="hero">
<div>
<h1>FLASH <span class="neon">DRINK</span></h1>
<p class="subtitle">Neon vibe minden ízben ⚡<br>Lightly Carbonated. Ultra Friss.</p>
<button class="btn">Kóstold meg 😌</button>
</div>
</section>

<section class="section">
<h2>Miért Flash Drink?</h2>
<div class="cards">
<div class="card"><h3>⚡ Energy Vibe</h3><p>Frissít, nem nehéz. Pörgős, de chill.</p></div>
<div class="card"><h3>💨 Lightly Carbonated</h3><p>Nem cola szint. Pont jó buborékok.</p></div>
<div class="card"><h3>❄ Cooling Effect</h3><p>Hűsítő érzet. Ultra friss.</p></div>
<div class="card"><h3>🍉 Neon Melon</h3><p>Dinnye + lime vibe.</p></div>
<div class="card"><h3>🍓 Neon Berry</h3><p>Áfonya + málna vibe.</p></div>
<div class="card"><h3>🍋 Neon Citrus</h3><p>Citrom + lime vibe.</p></div>
</div>
</section>

<section class="section shop">
<h2>Rendelj most!</h2>
<button>Neon Melon 😎</button>
<button>Neon Berry 🍓</button>
<button>Neon Citrus 🍋</button>
<p class="subtitle">Ez csak demo, de brutál menő lenne IRL 😏</p>
</section>

<footer>Flash Drink © Future Drink 😌⚡</footer>
</body>
</html>
