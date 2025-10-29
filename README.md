<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>[Your Name] — AI/ML Systems Engineer</title>
  <meta name="description" content="AI/ML systems, multi-agent frameworks, developer tooling, and applied research." />
  <meta property="og:title" content="[Your Name] — AI/ML Systems Engineer" />
  <meta property="og:description" content="AI/ML systems, multi-agent frameworks, developer tooling, and applied research." />
  <meta name="theme-color" content="#0ea5e9" />
  <style>
    :root {
      --bg: #0b0c10;
      --bg-elev: #111318;
      --text: #e5e7eb;
      --muted: #9aa3af;
      --brand: #0ea5e9;
      --card: #0f1218;
      --border: #1f2430;
      --code: #0b1220;
      --shadow: 0 10px 30px rgba(0,0,0,.35);
    }
    @media (prefers-color-scheme: light) {
      :root {
        --bg: #f8fafc;
        --bg-elev: #ffffff;
        --text: #0f172a;
        --muted: #475569;
        --brand: #0ea5e9;
        --card: #ffffff;
        --border: #e5e7eb;
        --code: #f1f5f9;
        --shadow: 0 8px 24px rgba(2, 6, 23, .08);
      }
    }
    * { box-sizing: border-box; }
    html, body { margin: 0; padding: 0; }
    body {
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Inter, Helvetica, Arial, "Apple Color Emoji", "Segoe UI Emoji";
      background: radial-gradient(1200px 600px at 80% -10%, rgba(14,165,233,.12), transparent 60%),
                  radial-gradient(800px 800px at -10% 20%, rgba(99,102,241,.10), transparent 50%),
                  var(--bg);
      color: var(--text);
      line-height: 1.6;
    }
    a { color: var(--brand); text-decoration: none; }
    a:hover { text-decoration: underline; }
    .container {
      max-width: 980px;
      margin: 0 auto;
      padding: 32px 20px 80px;
    }
    header {
      display: grid;
      gap: 12px;
      padding: 28px 22px;
      border: 1px solid var(--border);
      border-radius: 18px;
      background: linear-gradient(180deg, var(--bg-elev), var(--card));
      box-shadow: var(--shadow);
    }
    .tag {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      font-size: 12px;
      color: var(--muted);
      padding: 6px 10px;
      border: 1px solid var(--border);
      border-radius: 999px;
      background: linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,0));
      width: max-content;
    }
    .title {
      font-size: clamp(28px, 4vw, 42px);
      line-height: 1.15;
      letter-spacing: -0.02em;
      margin: 0;
    }
    .subtitle { color: var(--muted); margin: 0; font-size: 16px; }
    .links { display: flex; flex-wrap: wrap; gap: 12px; margin-top: 8px; }
    .chip {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 8px 12px;
      border: 1px solid var(--border);
      border-radius: 12px;
      background: var(--bg-elev);
      box-shadow: var(--shadow);
      font-size: 14px;
    }
    .grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 24px;
      margin-top: 28px;
    }
    @media (min-width: 880px) {
      .grid { grid-template-columns: 1.1fr .9fr; gap: 28px; }
    }
    section {
      padding: 18px 22px;
      border: 1px solid var(--border);
      border-radius: 16px;
      background: var(--card);
      box-shadow: var(--shadow);
    }
    h2 {
      margin: 4px 0 12px;
      font-size: 20px;
      letter-spacing: .2px;
    }
    .item + .item { border-top: 1px dashed var(--border); padding-top: 14px; margin-top: 14px; }
    .item h3 { margin: 0 0 4px; font-size: 16px; }
    .meta {
      color: var(--muted);
      font-size: 13px;
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }
    ul { margin: 10px 0 0 18px; }
    li { margin: 6px 0; }
    .pill {
      display: inline-block;
      border: 1px solid var(--border);
      background: var(--bg-elev);
      border-radius: 999px;
      padding: 6px 10px;
      font-size: 12px;
      margin: 4px 6px 0 0;
      color: var(--muted);
    }
    code, .code {
      background: var(--code);
      padding: 2px 6px;
      border-radius: 6px;
      border: 1px solid var(--border);
      font-family: ui-monospace, SFMono-Regular, Menlo, Consolas, "Liberation Mono", monospace;
      font-size: .92em;
    }
    footer {
      color: var(--muted);
      font-size: 13px;
      margin-top: 26px;
      text-align: center;
    }
    .sr-only {
      position: absolute; width: 1px; height: 1px; padding: 0; margin: -1px;
      overflow: hidden; clip: rect(0,0,0,0); white-space: nowrap; border: 0;
    }
  </style>
</head>
<body>
  <div class="container">
    <header role="banner" aria-label="Intro">
      <span class="tag" aria-hidden="true">AI/ML Systems • Multi-Agent • Dev Tools</span>
      <h1 class="title">Hi, I’m <span style="color:var(--brand)">[Your Name]</span> — building AI/ML systems that scale</h1>
      <p class="subtitle">
        I design and ship production-ready AI platforms, multi-agent reasoning frameworks, and developer tooling—focused on reliability, cost, and real-world throughput.
      </p>
      <nav class="links" aria-label="Primary">
        <a class="chip" href="https://github.com/yourhandle" target="_blank" rel="noopener">GitHub</a>
        <a class="chip" href="https://www.linkedin.com/in/yourhandle" target="_blank" rel="noopener">LinkedIn</a>
        <a class="chip" href="mailto:you@example.com">you@example.com</a>
        <a class="chip" href="#projects">Projects</a>
        <a class="chip" href="#experience">Experience</a>
        <a class="chip" href="#education">Education</a>
      </nav>
    </header>

    <main class="grid" id="main" role="main">
      <!-- Left column -->
      <div>
        <section id="experience" aria-labelledby="exp-h">
          <h2 id="exp-h">Experience</h2>

          <div class="item">
            <h3>Agentico AI, Inc. — Software Engineer &amp; Cofounder</h3>
            <div class="meta">Madrid, Spain • Mar 2025 – Aug 2025</div>
            <ul>
              <li>Built a <span class="code">tree-structured LLM framework (Thread–Node)</span> for hierarchical context, workflow automation, and parallel multi-agent reasoning.</li>
              <li>Integrated <span class="code">LangGraph + RAG</span> with <span class="code">PostgreSQL / S3 / Chroma</span> to handle <strong>10M+ documents</strong> with minimal memory overhead.</li>
              <li>Designed modular agent pipelines for NL-to-workflow orchestration; parent threads coordinate specialized child nodes, improving throughput by <strong>65%</strong> and optimizing KV cache use.</li>
              <li>Deployed on <span class="code">AWS (EC2, S3, Terraform)</span> for real-time multi-threaded reasoning; reduced infra cost <strong>30%</strong> via resource-aware scaling.</li>
              <li>Led an engineering team (CMU, Tsinghua, Northwestern, UW–Madison). Awards: <strong>$10K</strong> total (Microsoft Datamellon AI Ignite 3rd, UChicago 3rd, Northwestern 2nd). Invited <em>OpenAI SolarFlow</em> talk.</li>
            </ul>
          </div>

          <div class="item">
            <h3>American Battery Solutions, Inc. — Software Engineer Intern (Full-time)</h3>
            <div class="meta">Lake Orion, Michigan, U.S. • Jan 2025 – Mar 2025</div>
            <ul>
              <li>Delivered a production-grade <strong>code intelligence &amp; auto-documentation</strong> platform across multi-repo codebases.</li>
              <li>Engineered an <span class="code">AST</span> pipeline (libCST + networkx) for dependencies, call graphs, and interface contracts; integrated with <span class="code">GitLab CI</span> to gate merges.</li>
              <li>Published a self-serve docs portal (<span class="code">FastAPI + Graphviz</span>) with continuous system diagrams; cut manual docs by <strong>85%</strong> and onboarding by <strong>60%</strong>.</li>
              <li>Hardened SDLC with shift-left checks &amp; traceability, improving review throughput and reducing rework.</li>
            </ul>
          </div>

          <div class="item">
            <h3>IsVision Technology Co., Ltd. — Software Engineer Intern (Full-time)</h3>
            <div class="meta">Shanghai, China • Jun 2024 – Sep 2024</div>
            <ul>
              <li>Built an <strong>AI-driven security/code reviewer</strong> (FastAPI, LiteLLM, GitLab webhooks) for 100+ CV repos, eliminating manual triage (~300+ hrs/week saved) and boosting vuln detection.</li>
              <li>Shipped a scalable <strong>self-RAG review service</strong> (LLaMA 3-70B + Chroma) for inline suggestions &amp; impact-based prioritization from commit diffs.</li>
              <li>Integrated reviewer as <span class="code">merge/commit gate</span> in GitLab CI; added high-throughput feedback loop with RabbitMQ, Redis, MongoDB.</li>
            </ul>
          </div>

          <div class="item">
            <h3>Computer Vision Center (CVC) — Research Assistant</h3>
            <div class="meta">Barcelona, Spain • Jun 2022 – Jan 2023</div>
            <ul>
              <li>Co-authored the <strong>MILL (Multi-Illumination Low-Light)</strong> dataset: 50 scenes × 11 light levels; DSLR + smartphone RAW with lux &amp; programmable-light metadata (1,100 images).</li>
              <li>Built capture/processing pipeline and splits; released 600×400 set and tiled full-HD DSLR variant (5.5K images); ensured non-overlapping content across splits.</li>
              <li>Benchmarked SOTA (Retinexformer, LLFormer, MirNet, KinD, SCI, RUAS, FourLLIE) via PSNR<sub>L</sub>/PSNR<sub>C</sub>, SSIM, E, NIQE/BRISQUE/NIMA.</li>
              <li>Proposed <strong>I-Retinexformer</strong> with latent-intensity supervision; up to +9 dB PSNR (DSLR) and +1 dB (smartphone); improved color fidelity. Submitted to AAAI.</li>
            </ul>
          </div>
        </section>

        <section id="projects" aria-labelledby="proj-h">
          <h2 id="proj-h">Selected Projects</h2>
          <div class="item">
            <h3>Weather Prediction Pipeline</h3>
            <div class="meta">Kafka • Spark • Cassandra • Docker</div>
            <p>Real-time ingestion and forecasting with a resilient, containerized data path.</p>
          </div>
          <div class="item">
            <h3>Intelligent Flock Simulation</h3>
            <div class="meta">Multi-agent systems</div>
            <p>Emergent behaviors and control policies for cooperative agent swarms.</p>
          </div>
          <div class="item">
            <h3>AI Recommender System App</h3>
            <div class="meta">React Native</div>
            <p>End-to-end mobile recommendations with model-driven UX.</p>
          </div>
          <div class="item">
            <h3>Chess via Q-learning</h3>
            <div class="meta">RL • Tabular Q-learning</div>
            <p>Environment design, reward shaping, and policy evaluation for a classic board domain.</p>
          </div>
        </section>
      </div>

      <!-- Right column -->
      <aside aria-label="About & Skills">
        <section id="about" aria-labelledby="about-h">
          <h2 id="about-h">About</h2>
          <p>I build AI/ML systems, multi-agent orchestration, and developer platforms. I like squeezing latency and cost without sacrificing reliability.</p>
          <div aria-label="Interests">
            <span class="pill">LLM systems</span>
            <span class="pill">Multi-agent orchestration</span>
            <span class="pill">Cache-aware inference</span>
            <span class="pill">RAG at scale</span>
            <span class="pill">Code intelligence</span>
            <span class="pill">Low-light vision</span>
          </div>
        </section>

        <section id="education" aria-labelledby="edu-h">
          <h2 id="edu-h">Education</h2>
          <div class="item">
            <h3>Carnegie Mellon University — M.S. ECE (Advanced AI/ML Systems)</h3>
            <div class="meta">Pittsburgh, PA • Jan 2026 – Dec 2027</div>
            <ul>
              <li>Focus: AI/ML systems, scalable inference, distributed training, systems for LLMs.</li>
              <li>CSRankings Global: <strong>#1 in Computer Science</strong>.</li>
            </ul>
          </div>
          <div class="item">
            <h3>University of Wisconsin–Madison — B.S. CS &amp; Data Science</h3>
            <div class="meta">Madison, WI • Jan 2023 – May 2025</div>
            <ul>
              <li>Projects: Weather Prediction (Kafka/Spark/Cassandra/Docker), Intelligent Flock Simulation, AI Recommender (React Native), Chess via Q-learning.</li>
            </ul>
          </div>
        </section>

        <section id="skills" aria-labelledby="skills-h">
          <h2 id="skills-h">Tech I Use</h2>
          <p><strong>Languages:</strong> Python, TypeScript/JavaScript, SQL</p>
          <p><strong>Infra &amp; Data:</strong> AWS (EC2, S3, Terraform), Kafka, Spark, Cassandra, PostgreSQL, MongoDB, Redis, RabbitMQ, Docker</p>
          <p><strong>ML/AI:</strong> LangGraph, RAG (Chroma/S3), LLaMA-family LLMs, classical ML, RL (Q-learning)</p>
          <p><strong>Dev &amp; Docs:</strong> FastAPI, Graphviz, GitLab CI, libCST, networkx</p>
        </section>

        <section id="honors" aria-labelledby="honors-h">
          <h2 id="honors-h">Honors &amp; Talks</h2>
          <ul>
            <li>Microsoft Datamellon AI Ignite — 3rd Place</li>
            <li>University of Chicago — 3rd Place</li>
            <li>Northwestern — 2nd Place</li>
            <li>Invited OpenAI SolarFlow presentation</li>
          </ul>
        </section>
      </aside>
    </main>

    <footer role="contentinfo">
      <p>&copy; <span id="year"></span> [Your Name]. Built for GitHub Pages.</p>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
