<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Krittika Biswas | Portfolio</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: "Poppins", sans-serif;
    }
    body {
      background: #f9fafc;
      color: #222;
      line-height: 1.6;
    }
    header {
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      padding: 40px;
      background: linear-gradient(135deg, #6c63ff, #48a9fe);
      color: white;
      text-align: center;
    }
    header h1 {
      font-size: 3rem;
      font-weight: 700;
      margin-bottom: 10px;
    }
    header p {
      font-size: 1.2rem;
      opacity: 0.9;
      max-width: 600px;
      margin-bottom: 20px;
    }
    header a {
      padding: 12px 24px;
      background: white;
      color: #333;
      text-decoration: none;
      border-radius: 8px;
      font-weight: 600;
      transition: 0.3s;
    }
    header a:hover {
      background: #eee;
    }

    section {
      padding: 80px 20px;
      max-width: 900px;
      margin: auto;
    }
    section h2 {
      font-size: 2rem;
      margin-bottom: 20px;
      text-align: center;
    }
    .about {
      text-align: center;
      font-size: 1.1rem;
      max-width: 700px;
      margin: auto;
    }

    .skills, .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      margin-top: 30px;
    }
    .card {
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.08);
      transition: 0.3s;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 6px 16px rgba(0,0,0,0.12);
    }

    footer {
      text-align: center;
      padding: 30px;
      margin-top: 40px;
      background: #f1f3f8;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>

  <header>
    <h1>Hi, I'm Krittika</h1>
    <p>A passionate learner exploring web development, coding, and creative tech. This is my modern single‑page portfolio built entirely with custom HTML & CSS.</p>
    <a href="#about">Explore my site ↓</a>
  </header>

  <section id="about">
    <h2>About Me</h2>
    <p class="about">I'm an IT student learning web development, JavaScript, Git, and software engineering. I love building clean interfaces, solving coding problems, and exploring new technologies.</p>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <div class="skills">
      <div class="card">HTML & CSS</div>
      <div class="card">JavaScript</div>
      <div class="card">Git & GitHub</div>
      <div class="card">C Programming</div>
      <div class="card">Problem Solving</div>
    </div>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="projects">
      <div class="card">• Portfolio Website<br>Modern clean personal site</div>
      <div class="card">• GitHub Pages Blog<br>Built with Jekyll + Markdown</div>
      <div class="card">• Coding Tasks<br>Algorithms & DSA practice</div>
    </div>
  </section>

  <section id="blog">
    <h2>Latest Blog Post</h2>
    <p style="text-align:center;">Your GitHub Pages blog posts will appear here automatically once integrated.</p>
  </section>

  <footer>
    © 2025 Krittika Biswas — All Rights Reserved
  </footer>

</body>
</html>
