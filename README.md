# Fundedfx
Ai
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Funded FX</title>
<style>
  :root { --bg:#0b0b0c; --card:#151517; --line:#26262a; --accent:#d4f77a; --muted:#9ca3af; }
  * { box-sizing:border-box; margin:0; font-family:system-ui,sans-serif; }
  body { background:var(--bg); color:#fff; display:flex; min-height:100vh; }
  .side { width:56px; border-right:1px solid var(--line); display:flex; flex-direction:column; align-items:center; padding:14px 0; gap:18px; }
  .logo { color:var(--accent); font-weight:700; }
  .ico { width:36px; height:36px; border-radius:10px; display:grid; place-items:center; color:var(--muted); }
  .ico.on { background:var(--card); color:var(--accent); }
  .main { flex:1; min-width:0; }
  .top { display:flex; gap:8px; align-items:center; padding:12px; border-bottom:1px solid var(--line); }
  .top input { flex:1; min-width:0; background:var(--card); border:1px solid var(--line); border-radius:99px; padding:9px 14px; color:#fff; }
  .btn { background:var(--accent); color:#000; border:0; border-radius:99px; padding:9px 14px; font-weight:600; font-size:13px; }
  .wrap { padding:16px; display:grid; gap:16px; }
  h1 { font-size:22px; } .sub { color:var(--muted); font-size:13px; margin-top:4px; }
  .card { background:var(--card); border:1px solid var(--line); border-radius:16px; padding:16px; }
  .eq { border-left:2px solid var(--accent); padding-left:10px; }
  .lbl { color:var(--muted); font-size:12px; } .big { font-size:24px; font-weight:600; margin-top:4px; }
  .grid { display:grid; grid-template-columns:1fr 1fr; gap:12px; }
  .empty { text-align:center; padding:40px 16px; }
  .empty p { color:var(--muted); font-size:13px; margin:6px 0 16px; }
  svg { width:100%; height:120px; margin-top:12px; }
</style>
</head>
<body>
  <aside class="side">
    <div class="logo">FX</div>
    <div class="ico on">⌂</div><div class="ico">▤</div>
    <div class="ico">↗</div><div class="ico">★</div><div class="ico">♥</div>
  </aside>

  <div class="main">
    <div class="top">
      <input placeholder="Search accounts, trades, payouts">
      <button class="btn">Start Challenge</button>
    </div>

    <div class="wrap">
      <div>
        <h1>Welcome back, Trader</h1>
        <p class="sub">Your trading hub at a glance.</p>
      </div>

      <div class="card">
        <div class="eq">
          <div class="lbl">Total equity</div>
          <div class="big">$0 <span class="lbl" style="color:var(--accent)">(+0.0%)</span></div>
        </div>
        <svg viewBox="0 0 300 100" preserveAspectRatio="none">
          <line x1="0" y1="50" x2="300" y2="50" stroke="#d4f77a" stroke-width="2"/>
        </svg>
      </div>

      <div class="grid">
        <div class="card"><div class="lbl">All accounts</div><div class="big">0</div></div>
        <div class="card"><div class="lbl">Active accounts</div><div class="big">0</div></div>
        <div class="card"><div class="lbl">Funded accounts</div><div class="big">0</div></div>
        <div class="card"><div class="lbl">Total payouts</div><div class="big">$0.00</div></div>
      </div>

      <div class="card empty">
        <strong>Start trading</strong>
        <p>Buy your first challenge to begin.</p>
        <button class="btn">Buy a challenge</button>
      </div>
    </div>
  </div>
</body>
</html>
