# Index.html
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>John Louise B. Ragot — Portfolio</title>
<meta name="description" content="Portfolio — John Louise B. Ragot (16) | Student" />
<style>
  /* Reset & utilities */
  :root{
    --bg1:#071025;
    --bg2:#071033;
    --card:#0b1220;
    --muted:#9aa7bf;
    --accent1:#4f46e5;
    --accent2:#06b6d4;
    --glass: rgba(255,255,255,0.03);
    --radius:14px;
  }
  *{box-sizing:border-box}
  html,body{height:100%;margin:0;font-family:Inter, "Segoe UI", Roboto, Arial, sans-serif;-webkit-font-smoothing:antialiased;}
  body{
    background: radial-gradient(1200px 400px at 10% 10%, rgba(79,70,229,0.12), transparent),
                radial-gradient(900px 300px at 90% 80%, rgba(6,182,212,0.06), transparent),
                linear-gradient(180deg,var(--bg1),var(--bg2));
    color:#e6eef8;
    padding:20px;
    display:flex;
    justify-content:center;
  }
  .wrap{width:100%;max-width:1100px;}

  /* header / hero */
  header{display:flex;gap:16px;align-items:center;justify-content:space-between;margin-bottom:20px}
  .brand{display:flex;gap:14px;align-items:center}
  .avatar{
    width:72px;height:72px;border-radius:14px;
    background:linear-gradient(135deg,var(--accent1),var(--accent2));
    display:flex;align-items:center;justify-content:center;font-weight:700;font-size:20px;color:white;
    box-shadow:0 8px 30px rgba(6,182,212,0.08);
    transform:translateY(0);
    transition:transform .35s cubic-bezier(.2,.9,.2,1);
  }
  .avatar:hover{transform:translateY(-6px) rotate(-2deg)}
  .name{line-height:1}
  .name h1{margin:0;font-size:1.2rem}
  .name p{margin:2px 0 0 0;color:var(--muted);font-size:0.95rem}

  /* nav simple */
  nav{display:flex;gap:10px}
  .btn{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:8px 12px;border-radius:12px;text-decoration:none;color:var(--muted);font-weight:600;font-size:0.9rem}
  .btn.primary{background:linear-gradient(90deg,var(--accent1),var(--accent2));color:white;border:0;box-shadow:0 8px 24px rgba(79,70,229,0.12)}

  /* hero card */
  .hero{
    display:grid;
    grid-template-columns:1fr 340px;
    gap:18px;
    margin-bottom:20px;
  }
  .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);padding:18px;border-radius:var(--radius);box-shadow:0 10px 30px rgba(2,6,23,0.6);backdrop-filter: blur(6px);}
  .intro h2{margin:0;font-size:1.6rem;letter-spacing:-0.5px}
  .intro p{margin:8px 0 0 0;color:var(--muted);line-height:1.5}
  .cta{display:flex;gap:10px;margin-top:12px}

  /* row */
  .row{display:grid;grid-template-columns:2fr 1fr;gap:18px}
  main{min-height:200px}
  h2.section{margin:0 0 12px 0;font-size:1.15rem}

  /* projects list */
  .projects{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:12px}
  .proj{padding:12px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.015), transparent);transition:transform .35s ease, box-shadow .35s ease}
  .proj:hover{transform:translateY(-6px);box-shadow:0 18px 40px rgba(2,6,23,0.6)}
  .proj img{width:100%;height:140px;object-fit:cover;border-radius:10px;margin-bottom:10px}

  /* skills */
  .skills{display:flex;flex-wrap:wrap;gap:8px}
  .skill{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);padding:8px 10px;border-radius:12px;color:var(--muted);font-weight:600}

  /* iframe embed area */
  .embed-wrap{border-radius:12px;overflow:hidden;border:1px solid rgba(255,255,255,0.04);background:#071022}
  .embed-cta{padding:10px;color:var(--muted);font-size:0.95rem}

  /* footer */
  footer{text-align:center;color:var(--muted);margin-top:20px;font-size:0.9rem}

  /* animations (simple) */
  .float{
    animation: floaty 6s ease-in-out infinite;
  }
  @keyframes floaty{
    0%{transform:translateY(0) rotate(0)}
    50%{transform:translateY(-8px) rotate(-1deg)}
    100%{transform:translateY(0) rotate(0)}
  }
  .fade-in{opacity:0;transform:translateY(8px);animation:in .8s forwards}
  .delay-1{animation-delay:.15s}
  .delay-2{animation-delay:.28s}
  @keyframes in{to{opacity:1;transform:none}}

  /* responsive */
  @media(max-width:980px){
    .hero{grid-template-columns:1fr}
    .row{grid-template-columns:1fr}
    nav{display:none}
  }

  /* small tweaks for mobile */
  @media(max-width:420px){
    .avatar{width:56px;height:56px;font-size:18px}
    .intro h2{font-size:1.25rem}
  }
</style>
</head>
<body>
  <!--
    INSTRUCTIONS:
    1) Save this file as index.html and upload to your GitHub repo root.
    2) On your phone: open GitHub in browser (Desktop site) -> Add file -> Create new file -> paste -> Commit.
    3) Enable: Repo Settings → Pages → Source: main branch / (root).
    4) The Google Drive embed uses your folder id; ensure the folder and files are shared "Anyone with the link can view".
  -->

  <div class="wrap">
    <header class="fade-in">
      <div class="brand">
        <div class="avatar float" id="avatar">JL</div>
        <div class="name">
          <h1>John Louise B. Ragot</h1>
          <p>16 years old • Full-time Student<br><small style="color:var(--muted)">Medina National Comprehensive High School</small></p>
        </div>
      </div>

      <nav>
        <a class="btn" href="#projects">Projects</a>
        <a class="btn" href="#about">About</a>
        <a class="btn primary" href="#contact">Contact</a>
      </nav>
    </header>

    <section class="hero">
      <div class="card intro fade-in delay-1">
        <h2>Hi — I'm John Louise.</h2>
        <p>I build visual materials and help people present ideas clearly — brochures, infographics, and short videos. I also coach basic fitness and enjoy editing photos and videos.</p>
        <div class="cta">
          <a class="btn primary" href="#projects">See my brochure & infographic</a>
          <a class="btn" href="#contact">Contact</a>
        </div>
      </div>

      <aside class="card fade-in delay-2">
        <strong style="display:block;margin-bottom:8px">Quick Info</strong>
        <div style="color:var(--muted);margin-bottom:10px">
          Age: 16<br>
          Student at Medina National Comprehensive High School<br>
        </div>

        <strong style="display:block;margin-top:6px">Skills</strong>
        <div class="skills" style="margin-top:8px">
          <div class="skill">Basic fitness coaching</div>
          <div class="skill">Photo editing</div>
          <div class="skill">Video editing</div>
        </div>

        <div style="margin-top:12px">
          <a class="btn" id="downloadResume" href="#" style="display:inline-block">Download Resume</a>
        </div>
      </aside>
    </section>

    <div class="row">
      <main class="card fade-in">
        <h2 class="section">Projects</h2>
        <p style="color:var(--muted);margin-top:0">Below are your brochure and infographics embedded from your Google Drive folder. If the folder fails to display in some browsers, a direct link is provided under each embed.</p>

        <!-- EMBED: Google Drive folder (uses folder id) -->
        <div style="margin-top:12px" class="embed-wrap">
          <!-- Replace the id below if different. Your folder id: 121ZpHLnBUqUWgPxoqhLGwElB1GEh6k-d -->
          <iframe
            src="https://drive.google.com/embeddedfolderview?id=121ZpHLnBUqUWgPxoqhLGwElB1GEh6k-d#grid"
            style="width:100%;height:520px;border:0"
            title="Brochure & Infographics"
            loading="lazy"></iframe>

          <div class="embed-cta" style="display:flex;justify-content:space-between;align-items:center;gap:12px;flex-wrap:wrap">
            <div>If you cannot see the folder above, open it directly:</div>
            <div style="margin-left:auto"><a class="btn" href="https://drive.google.com/drive/folders/121ZpHLnBUqUWgPxoqhLGwElB1GEh6k-d" target="_blank" rel="noreferrer">Open Drive Folder</a></div>
          </div>
        </div>

        <!-- Optional individual file embeds (fallback) -->
        <div style="margin-top:16px;display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:12px">
          <article class="proj">
            <img src="https://via.placeholder.com/800x500?text=Brochure+Preview" alt="Brochure preview">
            <h3>SeismoGuard Innovations — Brochure</h3>
            <p style="color:var(--muted);margin:6px 0 8px 0">Brochure showcasing SeismoGuard company overview and services.</p>
            <div style="display:flex;gap:8px">
              <a class="btn" href="https://drive.google.com/drive/folders/121ZpHLnBUqUWgPxoqhLGwElB1GEh6k-d" target="_blank">View / Download</a>
            </div>
          </article>

          <article class="proj">
            <img src="https://via.placeholder.com/800x500?text=Infographic+Preview" alt="Infographic preview">
            <h3>Bilingual Education — Infographic</h3>
            <p style="color:var(--muted);margin:6px 0 8px 0">Infographic and concept paper highlights for bilingual education project co-authored by John Louise.</p>
            <div style="display:flex;gap:8px">
              <a class="btn" href="https://drive.google.com/drive/folders/121ZpHLnBUqUWgPxoqhLGwElB1GEh6k-d" target="_blank">View / Download</a>
            </div>
          </article>
        </div>

      </main>

      <aside class="card fade-in" style="min-height:200px;">
        <h3 style="margin-top:0">About</h3>
        <p style="color:var(--muted)">I'm a full-time high school student focused on visual communications and community projects. I enjoy creating clear, attractive brochures and infographics, editing photos & videos, and helping others through basic fitness coaching sessions.</p>

        <h3 style="margin-top:14px">Contact</h3>
        <p style="color:var(--muted);margin:6px 0">Email: <a href="mailto:your.email@example.com" style="color:var(--accent2)">your.email@example.com</a></p>
        <p style="color:var(--muted);margin:6px 0">GitHub: <a href="https://github.com/yourusername" target="_blank" rel="noreferrer">github.com/yourusername</a></p>
        <p style="color:var(--muted);margin:6px 0">Location: Medina, Misamis Oriental</p>

        <div style="margin-top:12px">
          <a class="btn primary" href="#projects">View Projects</a>
        </div>
      </aside>
    </div>

    <footer>
      <div>© <span id="year"></span> John Louise B. Ragot — Made with ❤️ • Edit and deploy on GitHub Pages</div>
    </footer>
  </div>

<script>
  // small dynamic tweaks
  document.getElementById('year').textContent = new Date().getFullYear();
  // Avatar initials from name
  (function(){
    const name = 'John Louise B. Ragot';
    const initials = name.split(' ').map(s=>s[0]).slice(0,2).join('').toUpperCase();
    document.getElementById('avatar').textContent = initials;
  })();

  // Smooth scroll for internal links
  document.querySelectorAll('a[href^="#"]').forEach(a=>{
    a.addEventListener('click', e=>{
      e.preventDefault();
      const id = a.getAttribute('href').slice(1);
      const el = document.getElementById(id);
      if(el) el.scrollIntoView({behavior:'smooth', block:'start'});
    });
  });

  // Note: If your Drive folder is private, iframe will show permission prompt.
  // Make sure folder visibility: Anyone with the link -> Viewer.
</script>
</body>
</html>