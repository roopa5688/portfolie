# portfolie
This is my Task 2 project – Personal Portfolio Website from the Oasis Infobyte Web Development &amp; Designing Internship. Built using HTML and CSS, it includes an introduction with image, skills, resume link, and contact details. A clean, responsive layout to showcase my profile and abilities.
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Your Name — Portfolio</title>

  <!-- Google font (optional) -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

  <!-- Link to external CSS file -->
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <a href="#" class="brand">YourName</a>
      <nav class="nav">
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </nav>

      <button class="menu-toggle" aria-label="Open menu">☰</button>
    </div>
  </header>

  <main>
    <!-- Hero -->
    <section class="hero" id="home">
      <div class="container hero-grid">
        <div class="hero-text">
          <h1>Hi, I'm <span class="accent">Your Name</span></h1>
          <p class="lead">
            I build beautiful and user-friendly web experiences.
            I’m a frontend developer / designer based in City, Country.
          </p>
          <div class="hero-ctas">
            <a class="btn primary" href="#projects">See my work</a>
            <a class="btn ghost" href="#contact">Contact me</a>
          </div>
        </div>

        <div class="hero-card" aria-hidden="true">
          <!-- Placeholder avatar / illustration -->
          <div class="avatar-placeholder">Your Photo</div>
          <ul class="hero-meta">
            <li><strong>3+</strong> years experience</li>
            <li><strong>10+</strong> projects</li>
            <li><strong>Open</strong> to opportunities</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- About -->
    <section class="section" id="about">
      <div class="container">
        <h2>About me</h2>
        <p>
          Short intro about you. Mention your focus, technologies you enjoy and
          what problems you like to solve. Keep it 2–4 sentences.
        </p>

        <div class="about-grid">
          <div class="about-card">
            <h3>What I do</h3>
            <p>Designing interfaces, building interactive UIs, and shipping polished frontends.</p>
          </div>
          <div class="about-card">
            <h3>Tools</h3>
            <p>HTML, CSS, JavaScript, React, Git, Figma — and a love for accessibility.</p>
          </div>
          <div class="about-card">
            <h3>Process</h3>
            <p>Research → Design → Prototype → Build → Test. I value clarity and iteration.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Projects -->
    <section class="section" id="projects">
      <div class="container">
        <h2>Projects</h2>
        <p class="muted">A handful of projects I've shipped recently.</p>

        <div class="projects-grid">
          <!-- Project card -->
          <article class="project">
            <div class="project-thumb">Thumbnail</div>
            <div class="project-body">
              <h3>Project One</h3>
              <p class="muted">Short description — what it does and your role.</p>
              <div class="project-tags">
                <span>HTML</span><span>CSS</span><span>JavaScript</span>
              </div>
              <div class="project-links">
                <a href="#" target="_blank" rel="noopener">Live</a>
                <a href="#" target="_blank" rel="noopener">Code</a>
              </div>
            </div>
          </article>

          <article class="project">
            <div class="project-thumb">Thumbnail</div>
            <div class="project-body">
              <h3>Project Two</h3>
              <p class="muted">Short description — highlight the challenge or tech.</p>
              <div class="project-tags">
                <span>React</span><span>API</span>
              </div>
              <div class="project-links">
                <a href="#" target="_blank" rel="noopener">Live</a>
                <a href="#" target="_blank" rel="noopener">Code</a>
              </div>
            </div>
          </article>

          <article class="project">
            <div class="project-thumb">Thumbnail</div>
            <div class="project-body">
              <h3>Project Three</h3>
              <p class="muted">A one-liner about outcomes and impact.</p>
              <div class="project-tags">
                <span>Design</span><span>UX</span>
              </div>
              <div class="project-links">
                <a href="#" target="_blank" rel="noopener">Live</a>
                <a href="#" target="_blank" rel="noopener">Case study</a>
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>

    <!-- Skills -->
    <section class="section" id="skills">
      <div class="container">
        <h2>Skills</h2>
        <div class="skills-grid">
          <div class="skill">
            <h4>HTML & CSS</h4>
            <div class="meter"><span style="width:95%"></span></div>
          </div>
          <div class="skill">
            <h4>JavaScript</h4>
            <div class="meter"><span style="width:85%"></span></div>
          </div>
          <div class="skill">
            <h4>React</h4>
            <div class="meter"><span style="width:75%"></span></div>
          </div>
          <div class="skill">
            <h4>Design & UX</h4>
            <div class="meter"><span style="width:70%"></span></div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact -->
    <section class="section" id="contact">
      <div class="container contact-grid">
        <div>
          <h2>Contact</h2>
          <p>Interested in working together? Send me a message.</p>
          <ul class="contact-list">
            <li><strong>Email:</strong> <a href="mailto:your@email.com">your@email.com</a></li>
            <li><strong>Phone:</strong> +91 12345 67890</li>
            <li><strong>Location:</strong> City, Country</li>
          </ul>
        </div>

        <form class="contact-form" action="#" method="post" onsubmit="alert('Demo form — replace action with a real endpoint'); return false;">
          <label>
            <span>Name</span>
            <input type="text" name="name" required>
          </label>
          <label>
            <span>Email</span>
            <input type="email" name="email" required>
          </label>
          <label>
            <span>Message</span>
            <textarea name="message" rows="5" required></textarea>
          </label>
          <button class="btn primary" type="submit">Send message</button>
        </form>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container footer-inner">
      <p>© <span id="year"></span> Your Name. Built with ❤.</p>
      <div class="social">
        <a href="#" aria-label="GitHub">GitHub</a>
        <a href="#" aria-label="LinkedIn">LinkedIn</a>
        <a href="#" aria-label="Twitter">Twitter</a>
      </div>
    </div>
  </footer>

  <script>
    // small script: mobile menu toggle & set year
    document.querySelector('#year').textContent = new Date().getFullYear();
    const toggle = document.querySelector('.menu-toggle');
    const nav = document.querySelector('.nav');
    toggle?.addEventListener('click', () => {
      nav.classList.toggle('open');
    });

    // Smooth scroll for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(a => {
      a.addEventListener('click', function (e) {
        const href = this.getAttribute('href');
        if (href.length > 1) {
          e.preventDefault();
          document.querySelector(href)?.scrollIntoView({ behavior: 'smooth', block: 'start' });
          // close mobile menu if open
          if (nav.classList.contains('open')) nav.classList.remove('open');
        }
      });
    });
  </script>
</body>
</html>
/* Reset-ish */
* { box-sizing: border-box; margin: 0; padding: 0; }
html,body { height: 100%; font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; color: #1f2937; background: #fff; -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale; }

/* Variables */
:root{
  --container: 1100px;
  --accent: #2563eb; /* blue */
  --muted: #6b7280;
  --card: #f8fafc;
  --radius: 12px;
  --glass: rgba(255,255,255,0.6);
}

/* Layout helpers */
.container {
  width: min(var(--container), 92%);
  margin-left: auto;
  margin-right: auto;
}

/* Header */
.site-header {
  position: sticky;
  top: 0;
  background: linear-gradient(180deg, rgba(255,255,255,0.8), rgba(255,255,255,0.6));
  backdrop-filter: blur(6px);
  border-bottom: 1px solid rgba(30,41,59,0.05);
  z-index: 40;
}
.header-inner {
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:1rem;
  padding: 0.9rem 0;
}
.brand { font-weight:700; letter-spacing: -0.5px; text-decoration: none; color: inherit; }
.nav { display:flex; gap: 1rem; align-items:center; }
.nav a { text-decoration:none; color:var(--muted); padding: 0.45rem 0.5rem; border-radius:8px; font-weight:500; }
.nav a:hover { color: var(--accent); background: rgba(37,99,235,0.06); }

/* Mobile menu button */
.menu-toggle { display:none; background:none; border:0; font-size:1.2rem; cursor:pointer; }

/* Hero */
.hero { padding:3.2rem 0; }
.hero-grid { display:grid; grid-template-columns: 1fr 360px; gap:2.5rem; align-items:center; }
.hero-text h1 { font-size:2.05rem; margin-bottom:0.6rem; line-height:1.05; }
.lead { color: var(--muted); margin-bottom:1rem; font-size:1rem; }
.accent { color:var(--accent); }

.hero-ctas { display:flex; gap:0.75rem; margin-top:1rem; }
.btn { display:inline-block; padding:0.6rem 0.9rem; border-radius:10px; text-decoration:none; font-weight:600; }
.btn.primary { background:var(--accent); color:white; box-shadow: 0 6px 18px rgba(37,99,235,0.12); }
.btn.ghost { background:transparent; border: 1px solid rgba(15,23,42,0.06); color:var(--accent); }

/* Hero card */
.hero-card { background: linear-gradient(180deg,#ffffff,#fbfdff); border-radius: var(--radius); padding:1.4rem; box-shadow: 0 8px 30px rgba(15,23,42,0.06); text-align:center; }
.avatar-placeholder { height:150px; display:flex; align-items:center; justify-content:center; border-radius:12px; background:linear-gradient(180deg,#eef2ff,#fff); color:var(--muted); margin-bottom:1rem; font-weight:600; }
.hero-meta { list-style:none; display:flex; gap:0.5rem; justify-content:space-between; padding:0; margin:0; font-weight:600; color:var(--muted); }

/* Sections */
.section { padding: 3rem 0; }
.section h2 { font-size:1.35rem; margin-bottom:0.6rem; }
.muted { color: var(--muted); margin-bottom:1rem; }

/* About grid */
.about-grid { display:grid; grid-template-columns: repeat(3,1fr); gap:1rem; margin-top:1rem; }
.about-card { background: var(--card); padding:1rem; border-radius:12px; box-shadow: 0 6px 18px rgba(15,23,42,0.03); }

/* Projects */
.projects-grid { display:grid; grid-template-columns: repeat(3,1fr); gap:1rem; margin-top:1rem; }
.project { background:white; border-radius:12px; overflow:hidden; box-shadow: 0 10px 30px rgba(2,6,23,0.04); display:flex; flex-direction:column; }
.project-thumb { height:140px; display:flex; align-items:center; justify-content:center; background:linear-gradient(90deg,#eef2ff,#fff7ed); color:var(--muted); font-weight:700; }
.project-body { padding:1rem; flex:1; display:flex; flex-direction:column; gap:0.6rem; }
.project-tags { display:flex; gap:0.5rem; flex-wrap:wrap; margin-top:auto; }
.project-tags span { background:#f1f5f9; padding:0.25rem 0.5rem; border-radius:999px; font-size:0.8rem; color:var(--muted); }
.project-links { display:flex; gap:0.5rem; margin-top:0.5rem; }
.project-links a { text-decoration:none; font-weight:600; color:var(--accent); }

/* Skills */
.skills-grid { display:grid; grid-template-columns: repeat(2,1fr); gap:1rem; margin-top:1rem; }
.skill h4 { margin-bottom:0.4rem; }
.meter { height:10px; background:#eef2f6; border-radius:999px; overflow:hidden; }
.meter span { display:block; height:100%; background: linear-gradient(90deg,var(--accent), #60a5fa); }

/* Contact */
.contact-grid { display:grid; grid-template-columns: 1fr 420px; gap:2rem; align-items:start; }
.contact-list { list-style:none; margin-top:1rem; color:var(--muted); }
.contact-form { display:flex; flex-direction:column; gap:0.7rem; }
.contact-form label { display:flex; flex-direction:column; gap:0.3rem; font-weight:600; color:var(--muted); }
.contact-form input, .contact-form textarea {
  padding:0.6rem 0.75rem;
  border-radius:10px;
  border:1px solid #e6eef8;
  font-size:0.95rem;
  outline:none;
}
.contact-form input:focus, .contact-form textarea:focus { box-shadow: 0 4px 14px rgba(37,99,235,0.08); border-color: rgba(37,99,235,0.3); }

/* Footer */
.site-footer { border-top:1px solid rgba(30,41,59,0.05); padding:1.2rem 0; margin-top:2rem; }
.footer-inner { display:flex; gap:1rem; align-items:center; justify-content:space-between; }

/* Responsive */
@media (max-width: 980px){
  .hero-grid { grid-template-columns: 1fr; }
  .projects-grid { grid-template-columns: repeat(2,1fr); }
  .about-grid { grid-template-columns: repeat(2,1fr); }
  .skills-grid { grid-template-columns: 1fr; }
  .contact-grid { grid-template-columns: 1fr; }
}

@media (max-width: 700px){
  .header-inner { gap:0.5rem; }
  .nav { position: absolute; right: 1rem; top: 64px; background: white; padding:0.6rem; border-radius:10px; box-shadow: 0 12px 30px rgba(2,6,23,0.08); flex-direction:column; display:none; }
  .nav.open { display:flex; }
  .menu-toggle { display:block; }
  .projects-grid { grid-template-columns: 1fr; }
  .about-grid { grid-template-columns: 1fr; }
}

/* Small visual niceties */
a { color: inherit; }
h1,h2,h3,h4 { color: #0f172a; }





