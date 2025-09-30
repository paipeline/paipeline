<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Your Name — Designer & Art Director</title>
  <meta name="description" content="Portfolio of Your Name, a freelance designer & art director crafting brand identities, digital experiences, and campaigns." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg: #0f1216;
      --surface: #151a21;
      --text: #e7ecf1;
      --muted: #a7b0bb;
      --brand: #89b4ff; /* accent */
      --brand-2: #f5b6ff; /* gradient 2 */
      --ring: rgba(137,180,255,.35);
      --card: #0f1319;
      --maxw: 1140px;
      --radius: 16px;
      --shadow: 0 10px 30px rgba(0,0,0,.35);
    }
    @media (prefers-color-scheme: light){
      :root{
        --bg: #f7f8fb;
        --surface: #ffffff;
        --text: #0f1216;
        --muted: #4b5563;
        --brand: #3b82f6;
        --brand-2: #a855f7;
        --ring: rgba(59,130,246,.25);
        --card: #ffffff;
      }
    }

    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0; background:radial-gradient(1200px 800px at 80% -10%, rgba(137,180,255,.12), transparent 55%),
      radial-gradient(1000px 700px at 0% 0%, rgba(245,182,255,.10), transparent 45%), var(--bg);
      color:var(--text); font: 400 16px/1.6 "Inter", system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif;
    }
    a{color:inherit; text-decoration:none}
    img{max-width:100%; display:block; border-radius:12px}

    .container{max-width:var(--maxw); margin:0 auto; padding:0 24px}
    .pill{display:inline-flex; align-items:center; gap:8px; border:1px solid rgba(255,255,255,.12); padding:8px 12px; border-radius:999px; color:var(--muted); backdrop-filter: blur(8px)}
    .tag{display:inline-flex; padding:6px 10px; border-radius:999px; border:1px solid rgba(255,255,255,.12); color:var(--muted); font-size:12px}
    .btn{display:inline-flex; align-items:center; gap:10px; padding:12px 18px; border-radius:12px; border:1px solid rgba(255,255,255,.14); background:linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.03)); box-shadow: var(--shadow); transition:.2s transform, .2s box-shadow}
    .btn:hover{transform:translateY(-2px); box-shadow:0 14px 40px rgba(0,0,0,.45)}
    .btn.primary{border-color:transparent; background:linear-gradient(135deg, var(--brand), var(--brand-2)); color:#0b0e13; font-weight:600}

    /* Nav */
    .nav{position:sticky; top:0; z-index:40; backdrop-filter: blur(10px); background:linear-gradient(180deg, rgba(10,14,20,.6), rgba(10,14,20,0)); border-bottom:1px solid rgba(255,255,255,.06)}
    .nav .wrap{display:flex; align-items:center; justify-content:space-between; padding:14px 0}
    .logo{display:flex; align-items:center; gap:10px; font-weight:700}
    .logo .dot{width:12px; height:12px; border-radius:50%; background:linear-gradient(135deg, var(--brand), var(--brand-2)); box-shadow:0 0 0 6px var(--ring)}
    .nav a{color:var(--muted)}
    .nav .links{display:flex; gap:22px; align-items:center}

    /* Hero */
    .hero{padding:96px 0 56px}
    .hero .grid{display:grid; grid-template-columns: 1.2fr .8fr; gap:48px}
    h1{font-family:"Playfair Display", ui-serif, Georgia, serif; font-weight:700; letter-spacing:-.02em; font-size: clamp(36px, 5vw, 64px); line-height:1.05; margin:0 0 14px}
    .lede{color:var(--muted); font-size:18px}
    .heroCard{position:relative; background:linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.03)); border:1px solid rgba(255,255,255,.12); border-radius:24px; padding:22px; overflow:hidden}
    .heroCard::after{content:""; position:absolute; inset:-30% -20% auto auto; width:340px; height:340px; background:radial-gradient(closest-side, rgba(137,180,255,.25), transparent 70%); transform:translate(30%,-20%); filter: blur(20px); pointer-events:none}

    /* Sections */
    section{padding:64px 0}
    .section-head{display:flex; align-items:baseline; justify-content:space-between; gap:12px; margin-bottom:22px}
    .section-head h2{font-size: clamp(24px, 2.6vw, 36px); margin:0}
    .section-head p{margin:0; color:var(--muted)}

    /* Work Grid */
    .work-grid{display:grid; grid-template-columns: repeat(12, 1fr); gap:18px}
    .card{grid-column: span 6; background:var(--card); border:1px solid rgba(255,255,255,.10); border-radius:20px; overflow:hidden; transition:.25s transform, .25s box-shadow, .25s border-color}
    .card:hover{transform:translateY(-4px); border-color: rgba(137,180,255,.5); box-shadow:0 18px 40px rgba(0,0,0,.35)}
    .card .media{position:relative; aspect-ratio: 16/10; overflow:hidden}
    .card .body{padding:16px 16px 18px}
    .card h3{margin:0 0 6px; font-size:20px}
    .card .meta{display:flex; gap:8px; flex-wrap:wrap}
    .card .desc{color:var(--muted); margin:8px 0 0}
    .wide{grid-column: span 12}

    /* Services */
    .services{display:grid; grid-template-columns: repeat(3, 1fr); gap:18px}
    .service{background:var(--card); border:1px solid rgba(255,255,255,.10); border-radius:20px; padding:18px}
    .service h3{margin:0 0 8px}
    .service p{margin:0; color:var(--muted)}

    /* Testimonials */
    .testimonials{display:grid; grid-template-columns: repeat(2, 1fr); gap:18px}
    .quote{background:var(--card); border:1px solid rgba(255,255,255,.10); border-radius:20px; padding:22px; position:relative}
    .quote::before{content:"“"; position:absolute; left:14px; top:-8px; font: 700 84px/0 "Playfair Display", serif; color:rgba(255,255,255,.09)}
    .client{display:flex; align-items:center; gap:12px; margin-top:12px; color:var(--muted)}

    /* Process */
    .process{display:grid; grid-template-columns: repeat(4, 1fr); gap:18px}
    .step{background:var(--card); border:1px solid rgba(255,255,255,.10); border-radius:18px; padding:16px}
    .step .num{display:inline-block; font-weight:700; padding:4px 8px; border-radius:999px; background:linear-gradient(135deg, var(--brand), var(--brand-2)); color:#0b0e13; margin-bottom:8px}

    /* Contact */
    .contact{display:grid; grid-template-columns:1.1fr .9fr; gap:24px}
    .contact .panel{background:var(--card); border:1px solid rgba(255,255,255,.10); border-radius:22px; padding:18px}
    label{font-size:14px; color:var(--muted)}
    input, textarea{width:100%; padding:12px 14px; border-radius:12px; background:var(--surface); border:1px solid rgba(255,255,255,.10); color:var(--text); outline:none}
    input:focus, textarea:focus{border-color:var(--brand); box-shadow:0 0 0 6px var(--ring)}

    /* Footer */
    footer{padding:28px 0 72px; color:var(--muted)}
    .footer-grid{display:grid; grid-template-columns: 2fr 1fr 1fr; gap:18px}
    .social{display:flex; gap:12px}

    /* Responsive */
    @media (max-width: 920px){
      .hero .grid, .contact{grid-template-columns:1fr}
      .work-grid .card, .services,.testimonials,.process{grid-template-columns:1fr}
      .card{grid-column: span 12}
      .footer-grid{grid-template-columns:1fr}
    }
  </style>

  <!-- Social preview -->
  <meta property="og:title" content="Your Name — Designer & Art Director" />
  <meta property="og:description" content="Brand identity, campaigns, websites. Available for select collaborations." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="/assets/cover.jpg" />
  <meta name="twitter:card" content="summary_large_image" />

  <!-- Structured data for SEO -->
  <script type="application/ld+json">
  {
    "@context":"https://schema.org",
    "@type":"Person",
    "name":"Your Name",
    "jobTitle":"Designer & Art Director",
    "url":"https://yourusername.github.io/",
    "sameAs":["https://www.linkedin.com/in/yourhandle","https://www.instagram.com/yourhandle","https://www.behance.net/yourhandle"],
    "worksFor":{"@type":"Organization","name":"Freelance"}
  }
  </script>
</head>
<body>
  <!-- Nav -->
  <nav class="nav">
    <div class="container wrap">
      <a class="logo" href="#home" aria-label="Home">
        <span class="dot" aria-hidden="true"></span>
        <span>Your&nbsp;Name</span>
      </a>
      <div class="links">
        <a href="#work">Work</a>
        <a href="#services">Services</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
        <a class="btn" href="assets/Your_Name_CV.pdf" target="_blank" rel="noopener">Résumé</a>
        <a class="btn primary" href="mailto:hello@yourdomain.com">Let’s collaborate</a>
      </div>
    </div>
  </nav>

  <!-- Hero -->
  <header id="home" class="hero container">
    <div class="grid">
      <div>
        <span class="pill">Designer & Art Director · Remote / Barcelona</span>
        <h1>I design brands & campaigns that make people feel something.</h1>
        <p class="lede">Independent designer & art director helping startups and culture brands turn ideas into distinctive identities, websites, and experiences.</p>
        <div style="display:flex; gap:12px; margin-top:18px">
          <a class="btn primary" href="#work">See selected work</a>
          <a class="btn" href="#about">About me</a>
        </div>
      </div>
      <div>
        <div class="heroCard">
          <img src="assets/hero-shot.jpg" alt="Collage of brand, web and campaign work" />
          <div style="display:flex; gap:8px; margin-top:12px; flex-wrap:wrap">
            <span class="tag">Brand Identity</span>
            <span class="tag">Art Direction</span>
            <span class="tag">Web Design</span>
            <span class="tag">Campaign</span>
            <span class="tag">Packaging</span>
          </div>
        </div>
      </div>
    </div>
  </header>

  <!-- Work -->
  <section id="work" class="container">
    <div class="section-head">
      <h2>Selected Work</h2>
      <p>More on <a href="https://www.behance.net/" target="_blank" rel="noopener">Behance</a> · <a href="https://dribbble.com/" target="_blank" rel="noopener">Dribbble</a></p>
    </div>

    <div class="work-grid">
      <!-- Project 1 -->
      <a class="card wide" href="#" aria-label="Project: Aurora Beverages">
        <div class="media"><img src="assets/work-aurora.jpg" alt="Aurora Beverages branding mockups" /></div>
        <div class="body">
          <h3>Aurora Beverages — Global rebrand</h3>
          <div class="meta">
            <span class="tag">Identity</span>
            <span class="tag">Packaging</span>
            <span class="tag">Guidelines</span>
          </div>
          <p class="desc">A luminous system blending bold typography with iridescent gradients across 40+ SKUs.</p>
        </div>
      </a>

      <!-- Project 2 -->
      <a class="card" href="#" aria-label="Project: Northbound Ventures">
        <div class="media"><img src="assets/work-northbound.jpg" alt="Northbound website and deck" /></div>
        <div class="body">
          <h3>Northbound Ventures — Venture site</h3>
          <div class="meta"><span class="tag">Web</span><span class="tag">Art Direction</span></div>
          <p class="desc">Clean, investor-first storytelling with motion micro-interactions.</p>
        </div>
      </a>

      <!-- Project 3 -->
      <a class="card" href="#" aria-label="Project: Playfair Festival">
        <div class="media"><img src="assets/work-playfair.jpg" alt="Festival campaign visuals" /></div>
        <div class="body">
          <h3>Playfair Festival — 360° campaign</h3>
          <div class="meta"><span class="tag">Campaign</span><span class="tag">OOH</span></div>
          <p class="desc">City-wide launch with variable typography and a vibrant grid system.</p>
        </div>
      </a>

      <!-- Add more cards as needed -->
    </div>
  </section>

  <!-- Services -->
  <section id="services" class="container">
    <div class="section-head">
      <h2>Services</h2>
      <p>Flexible, project-based or retained.</p>
    </div>
    <div class="services">
      <div class="service">
        <h3>Brand Identity</h3>
        <p>Naming, strategy, logo, typography, color, design systems, guidelines.</p>
      </div>
      <div class="service">
        <h3>Art Direction</h3>
        <p>Campaign concepts, creative direction, photoshoots, motion, OOH.</p>
      </div>
      <div class="service">
        <h3>Digital & Web</h3>
        <p>Marketing sites, product UI, design systems, no-code builds (Webflow).</p>
      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about" class="container">
    <div class="section-head">
      <h2>About</h2>
      <p>10+ years across studios & in-house. Available worldwide.</p>
    </div>
    <div class="heroCard" style="padding:22px">
      <p>Hi, I’m <strong>Your Name</strong>. I partner with founders and teams to craft enduring brands and clear, delightful experiences. Previously at <em>Studio X</em> and <em>Agency Y</em>. My work has been recognized by XYZ Awards and featured in ABC Mag.</p>
      <p style="margin-top:12px">When not designing, I mentor on <a href="#">ADPList</a> and explore creative tech.</p>
      <div style="display:flex; gap:10px; margin-top:14px">
        <span class="tag">Available Q4</span>
        <span class="tag">Remote-friendly</span>
        <span class="tag">English · Español · 中文</span>
      </div>
    </div>
  </section>

  <!-- Testimonials -->
  <section class="container">
    <div class="section-head">
      <h2>Kind Words</h2>
      <p>Partners & clients</p>
    </div>
    <div class="testimonials">
      <div class="quote">
        <p>“A rare blend of strategic thinking and taste. Our rebrand paid for itself within the quarter.”</p>
        <div class="client">
          <img src="assets/face-1.jpg" width="40" height="40" alt="Client portrait" style="border-radius:999px"/>
          <span>Alex Rivera, CMO at Aurora</span>
        </div>
      </div>
      <div class="quote">
        <p>“Pinpoint direction and immaculate craft. The campaign landed flawlessly across channels.”</p>
        <div class="client">
          <img src="assets/face-2.jpg" width="40" height="40" alt="Client portrait" style="border-radius:999px"/>
          <span>Sofia Kim, Producer at Playfair</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Process -->
  <section class="container">
    <div class="section-head">
      <h2>Process</h2>
      <p>Clear steps. No drama.</p>
    </div>
    <div class="process">
      <div class="step"><span class="num">01</span><h3>Discover</h3><p class="desc">Goals, audience, audit, success metrics.</p></div>
      <div class="step"><span class="num">02</span><h3>Define</h3><p class="desc">Strategy, creative territories, moodboards.</p></div>
      <div class="step"><span class="num">03</span><h3>Design</h3><p class="desc">Concepts → system → guidelines.</p></div>
      <div class="step"><span class="num">04</span><h3>Deliver</h3><p class="desc">Handoff, QA, launch support.</p></div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="container">
    <div class="section-head">
      <h2>Let’s work together</h2>
      <p>Two ways to reach out</p>
    </div>
    <div class="contact">
      <div class="panel">
        <h3 style="margin-top:0">Project inquiry</h3>
        <p class="lede">Tell me about your goals, timeline, and budget. I respond within 2 business days.</p>
        <form name="contact" method="POST" data-netlify="true">
          <input type="hidden" name="form-name" value="contact" />
          <div style="display:grid; grid-template-columns:1fr 1fr; gap:12px; margin:12px 0">
            <div>
              <label for="name">Name</label>
              <input id="name" name="name" required />
            </div>
            <div>
              <label for="email">Email</label>
              <input id="email" name="email" type="email" required />
            </div>
            <div style="grid-column:1/-1">
              <label for="message">Project details</label>
              <textarea id="message" name="message" rows="5" required></textarea>
            </div>
            <div>
              <label for="budget">Budget</label>
              <input id="budget" name="budget" placeholder="€5k–€20k" />
            </div>
            <div>
              <label for="timeline">Timeline</label>
              <input id="timeline" name="timeline" placeholder="e.g. November–January" />
            </div>
          </div>
          <button class="btn primary" type="submit">Send inquiry</button>
        </form>
      </div>
      <div class="panel">
        <h3 style="margin-top:0">Elsewhere</h3>
        <p>Prefer email? <a href="mailto:hello@yourdomain.com">hello@yourdomain.com</a></p>
        <div class="social" style="margin-top:10px">
          <a class="btn" href="https://www.linkedin.com/in/yourhandle" target="_blank" rel="noopener">LinkedIn</a>
          <a class="btn" href="https://www.instagram.com/yourhandle" target="_blank" rel="noopener">Instagram</a>
          <a class="btn" href="https://www.behance.net/yourhandle" target="_blank" rel="noopener">Behance</a>
        </div>
      </div>
    </div>
  </section>

  <footer class="container">
    <div class="footer-grid">
      <div>
        <div class="logo"><span class="dot" aria-hidden="true"></span><span>Your Name</span></div>
        <p style="margin-top:8px">Available for select projects and collaborations. Based in Barcelona · working worldwide.</p>
      </div>
      <div>
        <h4>Contact</h4>
        <p class="muted"><a href="mailto:hello@yourdomain.com">hello@yourdomain.com</a></p>
      </div>
      <div>
        <h4>Credits</h4>
        <p class="muted">© <span id="y"></span> Your Name. Built with ❤ on GitHub Pages.</p>
      </div>
    </div>
  </footer>

  <script>
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>
