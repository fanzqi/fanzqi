<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Welcome — Zulfan Syafiqi</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&family=Roboto+Mono:wght@400;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; /* deep navy */
      --card:#0b1220;
      --glass: rgba(255,255,255,0.04);
      --accent-1: #00d4ff;
      --accent-2: #7c4dff;
      --muted: #9aa4b2;
      --glass-border: rgba(255,255,255,0.06);
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial}
    body{
      background: radial-gradient(1200px 600px at 10% 10%, rgba(124,77,255,0.12), transparent 6%),
                  radial-gradient(900px 400px at 90% 90%, rgba(0,212,255,0.06), transparent 6%),
                  var(--bg);
      color:#e6eef6;
      display:flex;align-items:center;justify-content:center;padding:48px;
    }
    .card{
      width:min(880px,96%);
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border:1px solid var(--glass-border);
      border-radius:18px;
      padding:36px;
      display:grid;grid-template-columns:120px 1fr;gap:28px;align-items:center;backdrop-filter: blur(6px);
      box-shadow: 0 10px 30px rgba(2,6,23,0.6);
    }
    .avatar{
      width:120px;height:120px;border-radius:14px;overflow:hidden;border:1px solid rgba(255,255,255,0.04);display:flex;align-items:center;justify-content:center;background:linear-gradient(135deg,var(--accent-1),var(--accent-2));
    }
    .avatar img{width:100%;height:100%;object-fit:cover}
    .main h1{margin:0;font-size:28px;letter-spacing:-0.4px;font-weight:800}
    .subline{display:flex;gap:12px;align-items:center;margin-top:6px}
    .wave{width:44px;height:44px;border-radius:10px;background:linear-gradient(90deg,var(--accent-1),var(--accent-2));display:inline-flex;align-items:center;justify-content:center}
    .wave img{width:34px;height:34px}

    /* typing effect */
    .typing{font-family:'Roboto Mono', monospace;font-weight:700;font-size:18px;color:var(--accent-1);margin-top:8px;white-space:nowrap;overflow:hidden;border-right:2px solid rgba(255,255,255,0.06);width:0;animation:typing 3.6s steps(30,end) 0.6s forwards, blink 1s step-end infinite alternate;}
    @keyframes typing{
      to{width:26ch}
    }
    @keyframes blink{50%{border-color:transparent}}

    .desc{margin-top:16px;color:var(--muted);line-height:1.5}
    .actions{display:flex;gap:12px;margin-top:20px}
    .btn{padding:10px 14px;border-radius:10px;font-weight:600;text-decoration:none;border:1px solid transparent;background:transparent;color:var(--accent-1);display:inline-flex;gap:10px;align-items:center}
    .btn.secondary{color:var(--muted);border:1px solid rgba(255,255,255,0.03)}
    .meta{margin-left:auto;color:var(--muted);font-size:13px}

    .links{display:flex;gap:10px;margin-top:18px}
    .chip{padding:8px 10px;border-radius:10px;background:var(--glass);border:1px solid rgba(255,255,255,0.02);font-weight:600;font-size:13px;color:#dbe9ff}

    /* responsive */
    @media (max-width:640px){
      .card{grid-template-columns:72px 1fr;padding:22px}
      .avatar{width:72px;height:72px;border-radius:12px}
      .typing{font-size:15px}
    }
  </style>
</head>
<body>
  <div class="card" role="region" aria-label="Welcome card">
    <div class="avatar" title="Zulfan Syafiqi">
      <!-- If you have a photo, replace src with your image URL -->
      <img src="https://avatars.dicebear.com/api/identicon/Zulfan.svg" alt="avatar">
    </div>
    <div class="main">
      <div style="display:flex;align-items:center;gap:12px">
        <h1>Zulfan Syafiqi</h1>
        <div class="wave" aria-hidden="true">
          <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" alt="wave">
        </div>
        <div class="meta">San Francisco · Developer · Open to collaborations</div>
      </div>

      <div class="subline">
        <div class="typing">Hi, I build clean apps & delightful UX — welcome!</div>
      </div>

      <p class="desc">Profesional greeting card yang bersih, modern, dan siap dipakai di README atau halaman profil. Menggunakan tipografi modern, animasi tipis, dan palet warna gradien untuk kesan teknologi & elegan.</p>

      <div class="links" aria-hidden="false">
        <a class="chip" href="#">💼 Portfolio</a>
        <a class="chip" href="#">📄 Resume</a>
        <a class="chip" href="#">📫 Contact</a>
      </div>

      <div class="actions">
        <a class="btn" href="#">⭐ GitHub</a>
        <a class="btn secondary" href="#">🔗 LinkedIn</a>
      </div>
    </div>
  </div>
</body>
</html>
