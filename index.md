---
title: "Krittika Biswas — Portfolio"
layout: null
---

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="Krittika Biswas — student, developer, creative. Portfolio & blog." />
  <title>Krittika Biswas — Portfolio Blog</title>

  <!-- Google font (optional) -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa4b2; --accent:#7c5cff; --glass: rgba(255,255,255,0.06);
      --light-bg:#f8fafc; --light-card:#ffffff; --light-text:#0a0a0a;
    }
    /* dark-mode default; toggle will add .light on body */
    html,body{height:100%}
    body{
      margin:0; font-family:"Poppins",system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      background: linear-gradient(180deg, var(--bg), #081021 60%);
      color:#e6eef8; -webkit-font-smoothing:antialiased; line-height:1.5;
    }
    .light body{ background: var(--light-bg); color: var(--light-text); }

    /* layout */
    .wrap{max-width:980px;margin:0 auto;padding:28px}
    header.hero{
      display:flex; gap:32px; align-items:center; padding:48px 0;
      min-height:72vh;
    }
    .hero-left{flex:1}
    .hero-right{width:220px; display:flex; justify-content:center; align-items:center}
    .avatar{
      width:180px;height:180px;border-radius:50%;overflow:hidden;
      border:6px solid rgba(255,255,255,0.06); box-shadow:0 10px 30px rgba(2,6,23,0.6);
      transform:translateY(0); transition:transform .6s cubic-bezier(.2,.9,.3,1);
      background: linear-gradient(135deg, rgba(124,92,255,0.12), rgba(72,169,254,0.08));
    }
    .avatar img{width:100%;height:100%;object-fit:cover; display:block}

    h1{font-size:2.25rem; margin:0 0 8px; font-weight:700; letter-spacing:-0.02em}
    p.lead{margin:0 0 18px; color:var(--muted); max-width:56ch}

    .cta{display:inline-flex; gap:12px; align-items:center}
    .btn{
      padding:10px 16px; border-radius:10px; background:linear-gradient(90deg,var(--accent), #4fb1ff);
      color:white; text-decoration:none; font-weight:600; box-shadow:0 8px 20px rgba(124,92,255,0.14);
      transition: transform .2s, box-shadow .2s;
    }
    .btn.secondary{ background: transparent; border:1px solid rgba(255,255,255,0.06); color: #cfe6ff }

    .btn:hover{ transform: translateY(-4px); box-shadow:0 18px 40px rgba(76,64,255,0.14) }

    /* cards */
    .grid{display:grid; gap:20px; grid-template-columns: repeat(auto-fit, minmax(240px,1fr)); margin-top:26px}
    .card{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:12px; padding:18px; box-shadow: 0 6px 20px rgba(2,6,23,0.5);
      transition: transform .35s ease, box-shadow .35s ease;
      border:1px solid rgba(255,255,255,0.03);
    }
    .card:hover{ transform: translateY(-8px); box-shadow: 0 20px 50px rgba(2,6,23,0.6) }

    .muted{color:var(--muted); font-size:0.95rem}

    /* projects */
    .proj-title{font-weight:600; margin-bottom:6px}
    .proj-links a{display:inline-block;margin-right:10px;font-size:0.9rem;color:#dbeafe;text-decoration:none}
    .proj-links a:hover{text-decoration:underline}

    /* nav + topbar */
    nav.topbar{position:sticky; top:10px; display:flex; justify-content:space-between; align-items:center; margin-bottom:8px; z-index:40}
    .brand{font-weight:700;color:var(--accent)}
    .navlinks{display:flex; gap:12px; align-items:center}
    .navlinks a{color:inherit;text-decoration:none;padding:8px;border-radius:8px}
    .navlinks a:hover{background:rgba(255,255,255,0.03)}

    /* footer */
    footer{margin:48px 0 18px; color:var(--muted); text-align:center; font-size:0.95rem}

    /* animations */
    .reveal{opacity:0; transform: translateY(18px); transition: opacity .7s ease, transform .7s cubic-bezier(.2,.9,.3,1)}
    .reveal.visible{opacity:1; transform: translateY(0)}

    /* dark/light adjustments */
    .light .card{ background: linear-gradient(180deg,#fff,#fbfbff); border:1px solid rgba(10,10,10,0.04); box-shadow:0 8px 20px rgba(8,12,20,0.04) }
    .light .muted{ color:#6b7280 }

    /* small screens */
    @media (max-width:720px){
      header.hero{ flex-direction:column; text-align:center }
      .hero-right{ width:160px }
      h1{ font-size:1.6rem }
    }

  </style>
</head>
<body>

  <div class="wrap">

    <!-- top nav -->
    <nav class="topbar">
      <div class="brand">Krittika • dev</div>
      <div class="navlinks">
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#blog">Blog</a>
        <button id="themeToggle" class="btn secondary" title="Toggle light/dark">Light</button>
      </div>
    </nav>

    <!-- hero -->
    <header class="hero">
      <div class="hero-left">
        <h1 class="reveal">Hi — I’m <span style="color:var(--accent)">Krittika</span></h1>
        <p class="lead reveal" style="transition-delay:.05s">
          IT student • web dev learner • problem solver. I build small tools, integrate ends, and design clean interfaces.
        </p>

        <div class="cta reveal" style="transition-delay:.12s">
          <a class="btn" href="#projects">See Projects</a>
          <a class="btn secondary" href="#blog">Read Blog</a>
        </div>

        <div class="grid" style="margin-top:22px">
          <div class="card reveal" style="transition-delay:.18s">
            <div class="muted">Location</div>
            <div style="font-weight:600;margin-top:8px">Kolkata, India</div>
          </div>
          <div class="card reveal" style="transition-delay:.22s">
            <div class="muted">Role</div>
            <div style="font-weight:600;margin-top:8px">Student • Full Stack Web Dev</div>
          </div>
        </div>
      </div>

      <div class="hero-right">
        <div class="avatar reveal" style="transition-delay:.25s">
          <!-- Put your image at assets/images/logo.jpg -->
          <img src="/assets/images/photo.jpg" alt="Krittika photo" />
        </div>
      </div>
    </header>

    <!-- about -->
    <section id="about">
      <h2 class="reveal">About</h2>
      <p class="about reveal" style="transition-delay:.05s">
        I’m a final-year IT undergad diving deep into Wwb 3. I have a special keen for Git and algorithms, and I love building clean UI and learning new technologies.
      </p>
    </section>

    <!-- skills -->
    <section id="skills">
      <h2 class="reveal">Skills</h2>
      <div class="grid">
        <div class="card reveal"><strong>HTML & CSS</strong><div class="muted">Responsive layouts, flexbox, grid</div></div>
        <div class="card reveal"><strong>JavaScript</strong><div class="muted">DOM, ES6, small interactions</div></div>
        <div class="card reveal"><strong>Git & GitHub</strong><div class="muted">Repos, Pages, PRs</div></div>
        <div class="card reveal"><strong>C Programming</strong><div class="muted">Foundations & DSA practice</div></div>
      </div>
    </section>

    <!-- projects -->
    <section id="projects">
      <h2 class="reveal">Projects</h2>

      <div class="grid">
        <!-- Edit these cards: replace hrefs with your actual repo URLs -->
        <div class="card reveal">
          <div class="proj-title">Portfolio Website</div>
          <div class="muted">Modern single-page portfolio</div>
          <div class="proj-links" style="margin-top:10px">
            <a href="https://github.com/krittikabiswas/skills-github-pages" target="_blank" rel="noopener">Repo</a>
            <a href="https://krittikabiswas.github.io/skills-github-pages/" target="_blank" rel="noopener">Live</a>
          </div>
        </div>

        <div class="card reveal">
          <div class="proj-title">GitHub Pages Blog</div>
          <div class="muted">Jekyll + Markdown blog</div>
          <div class="proj-links" style="margin-top:10px">
            <a href="https://github.com/krittikabiswas/skills-github-pages" target="_blank" rel="noopener">Repo</a>
          </div>
        </div>

        <div class="card reveal">
          <div class="proj-title">DSA Practice</div>
          <div class="muted">Algorithms & problem solutions</div>
          <div class="proj-links" style="margin-top:10px">
            <!-- Replace with your actual DSA repo -->
            <a href="https://github.com/krittikabiswas/YOUR-DSA-REPO" target="_blank" rel="noopener">Repo</a>
          </div>
        </div>
      </div>
    </section>

    <!-- blog -->
    <section id="blog">
      <h2 class="reveal">Latest blog post</h2>
      <div class="card reveal" style="margin-top:16px">
        <div class="muted">Your Jekyll posts (from <code>_posts/</code>) will appear here automatically. Click below to open the _posts folder in your repo.</div>
        <div style="margin-top:12px">
          <a class="btn" href="https://github.com/krittikabiswas/skills-github-pages/tree/main/_posts" target="_blank">Open _posts</a>
        </div>
      </div>
    </section>

    <footer>
      © 2025 <strong>Krittika Biswas</strong> — Built with ❤️ • <a href="https://github.com/krittikabiswas" target="_blank" rel="noopener">@krittikabiswas</a>
    </footer>

  </div>

  <script>
    // reveal on scroll
    const revealEls = document.querySelectorAll('.reveal');
    const io = new IntersectionObserver((entries)=>{
      entries.forEach(e=>{
        if(e.isIntersecting) e.target.classList.add('visible');
      });
    }, {threshold:0.12});
    revealEls.forEach(el=>io.observe(el));

    // smooth scroll for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        e.preventDefault();
        const t = document.querySelector(a.getAttribute('href'));
        if(t) t.scrollIntoView({behavior:'smooth', block:'start'});
      });
    });

    // light/dark toggle (stores in localStorage)
    const toggle = document.getElementById('themeToggle');
    const root = document.documentElement;
    const setLight = (on) => {
      if(on){
        document.body.classList.add('light'); toggle.textContent='Dark';
      } else {
        document.body.classList.remove('light'); toggle.textContent='Light';
      }
      localStorage.setItem('lightMode', on?'1':'0');
    };
    // init from saved
    setLight(localStorage.getItem('lightMode') === '1');

    toggle.addEventListener('click', ()=>{
      setLight(!document.body.classList.contains('light'));
    });

    // tiny avatar hover effect
    const avatar = document.querySelector('.avatar');
    if(avatar){
      avatar.addEventListener('mouseenter', ()=> avatar.style.transform='translateY(-6px) scale(1.02)');
      avatar.addEventListener('mouseleave', ()=> avatar.style.transform='translateY(0) scale(1)');
    }
  </script>

</body>
</html>
