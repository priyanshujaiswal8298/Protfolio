<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Priyanshu Jaiswal — Portfolio</title>
  <meta name="description" content="Priyanshu Jaiswal | Puzzle creator, gamer & app developer" />
  <link rel="icon" href="data:;base64,iVBORw0KGgo=" />
  <style>
    :root{ --bg:#0f1724; --card:#0b1220; --muted:#94a3b8; --accent:#ff6b6b; --glass: rgba(255,255,255,0.03); }
    *{box-sizing:border-box} body{margin:0;font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;color:#e6eef8;background:linear-gradient(180deg,#071126 0%, #08111b 60%);min-height:100vh;display:flex;align-items:center;justify-content:center;padding:28px}
    .wrap{width:980px;max-width:100%;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:14px;padding:28px;box-shadow:0 8px 30px rgba(2,6,23,0.6);}
    header{display:flex;gap:20px;align-items:center}
    .avatar{width:110px;height:110px;border-radius:12px;background:linear-gradient(135deg,#1f2937,#111827);display:flex;align-items:center;justify-content:center;font-weight:700;color:#fff;font-size:28px;letter-spacing:1px}
    h1{margin:0;font-size:26px}
    .tag{color:var(--accent);font-weight:600}
    p.lead{margin:8px 0 0;color:var(--muted)}
    .grid{display:grid;grid-template-columns:2fr 1fr;gap:18px;margin-top:20px}
    .card{background:var(--card);padding:16px;border-radius:12px;box-shadow:inset 0 1px 0 rgba(255,255,255,0.02)}
    .section-title{font-weight:700;margin:0 0 10px}
    ul.skills{list-style:none;padding:0;margin:0;display:flex;flex-wrap:wrap;gap:8px}
    ul.skills li{background:var(--glass);padding:8px 10px;border-radius:8px;color:var(--muted);font-weight:600}
    .projects .proj{border-radius:10px;padding:12px;margin-bottom:10px;background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.00))}
    .contact-row{display:flex;flex-direction:column;gap:8px}
    a.btn{display:inline-block;padding:10px 14px;border-radius:10px;background:linear-gradient(90deg,var(--accent),#ff8a8a);color:white;text-decoration:none;font-weight:700}
    footer{margin-top:18px;text-align:center;color:var(--muted);font-size:13px}
    @media(max-width:720px){.grid{grid-template-columns:1fr}.avatar{width:88px;height:88px}}
  </style>
</head>
<body>
  <main class="wrap">
    <header>
      <div class="avatar">PJ</div>
      <div>
        <h1>Priyanshu Jaiswal <span class="tag">— Gaming · Puzzle Creator · App Dev</span></h1>
        <p class="lead">Hi, I’m Priyanshu Jaiswal! I love gaming, creating puzzles, and trying new tech ideas. I believe in learning something new every day and sharing it with others.</p>
        <div style="margin-top:10px;display:flex;gap:10px;align-items:center">
          <a class="btn" href="#contact">Contact Me</a>
          <a href="#projects" class="btn" style="background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted);font-weight:700">Projects</a>
        </div>
      </div>
    </header>

    <div class="grid">
      <section class="card">
        <h3 class="section-title">About</h3>
        <p>I build fun and educational things — puzzles, Android apps and small games. I enjoy making ideas into working projects and sharing them with the world.</p>

        <h3 class="section-title" style="margin-top:14px">Skills</h3>
        <ul class="skills">
          <li>Puzzle Making</li>
          <li>Android App Dev</li>
          <li>Game Development</li>
          <li>Web Development</li>
          <li>Video Editing</li>
          <li>Problem Solving</li>
        </ul>

        <h3 class="section-title" style="margin-top:14px">Projects</h3>
        <div class="projects">
          <div class="proj"><strong>Priyanshupuzzle</strong> — A puzzle & quiz website I created to share custom puzzles and brainteasers.</div>
          <div class="proj"><strong>Learning Buddy</strong> — A Duolingo-like multilingual learning app (Android APK).</div>
          <div class="proj"><strong>ASSINEX</strong> — A stealth-action Android game prototype.</div>
        </div>
      </section>

      <aside class="card">
        <h3 class="section-title">Contact</h3>
        <div class="contact-row">
          <div><strong>Email:</strong> <a href="mailto:jaiswalgaming8298@gmail.com">jaiswalgaming8298@gmail.com</a></div>
          <div><strong>Phone:</strong> <a href="tel:+918298740711">+91 8298740711</a></div>
          <div style="margin-top:8px"><strong>Social:</strong> <a href="https://github.com/priyanshujaiswal8298" target="_blank">GitHub</a> • <a href="#">Instagram</a></div>
        </div>

        <h3 class="section-title" style="margin-top:12px">Quick actions</h3>
        <div style="display:flex;flex-direction:column;gap:8px;margin-top:8px">
          <a class="btn" href="mailto:jaiswalgaming8298@gmail.com">Email Me</a>
          <a class="btn" href="tel:+918298740711">Call</a>
        </div>
      </aside>
    </div>

    <footer>
      © <span id="year"></span> Priyanshu Jaiswal — Built with ❤️
    </footer>
  </main>

  <script>
    // small script: set year + smooth scroll
    document.getElementById('year').textContent = new Date().getFullYear();
    document.querySelectorAll('a[href^="#"]').forEach(a=>{a.addEventListener('click', e=>{e.preventDefault();document.querySelector(a.getAttribute('href')).scrollIntoView({behavior:'smooth'});});});
  </script>
</body>
</html>
