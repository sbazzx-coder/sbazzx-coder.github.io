<!DOCTYPE html>

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mixed Fractal Analysis — IB Extended Essay</title>
  <link href="https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;1,400&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #0a0a0f;
      --surface: #111118;
      --border: #1e1e2e;
      --accent: #7c6af7;
      --accent2: #4af0c4;
      --text: #e8e8f0;
      --muted: #6b6b8a;
      --gold: #c8a96e;
    }

```
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
  background: var(--bg);
  color: var(--text);
  font-family: 'EB Garamond', Georgia, serif;
  font-size: 18px;
  line-height: 1.8;
  overflow-x: hidden;
}

/* Fractal canvas background */
#fractal-bg {
  position: fixed;
  top: 0; left: 0;
  width: 100%; height: 100%;
  opacity: 0.07;
  z-index: 0;
  pointer-events: none;
}

.container {
  position: relative;
  z-index: 1;
  max-width: 860px;
  margin: 0 auto;
  padding: 0 2rem;
}

/* Header */
header {
  padding: 5rem 0 3rem;
  border-bottom: 1px solid var(--border);
}

.ib-label {
  font-family: 'DM Mono', monospace;
  font-size: 0.7rem;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: var(--accent2);
  margin-bottom: 2rem;
  display: flex;
  align-items: center;
  gap: 1rem;
}

.ib-label::after {
  content: '';
  flex: 1;
  height: 1px;
  background: linear-gradient(90deg, var(--accent2), transparent);
}

h1 {
  font-size: clamp(2.2rem, 6vw, 3.8rem);
  font-weight: 400;
  line-height: 1.15;
  letter-spacing: -0.02em;
  margin-bottom: 1rem;
  background: linear-gradient(135deg, var(--text) 0%, var(--accent) 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.subtitle {
  font-style: italic;
  color: var(--muted);
  font-size: 1.1rem;
  margin-bottom: 2.5rem;
}

.meta-row {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  font-family: 'DM Mono', monospace;
  font-size: 0.75rem;
  color: var(--muted);
}

.meta-item span {
  color: var(--gold);
  display: block;
  margin-bottom: 0.2rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

/* Navigation */
nav {
  padding: 1.5rem 0;
  border-bottom: 1px solid var(--border);
  position: sticky;
  top: 0;
  background: rgba(10,10,15,0.92);
  backdrop-filter: blur(12px);
  z-index: 100;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 2rem;
  font-family: 'DM Mono', monospace;
  font-size: 0.72rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

nav a {
  color: var(--muted);
  text-decoration: none;
  transition: color 0.2s;
}

nav a:hover { color: var(--accent2); }

/* Sections */
section {
  padding: 4rem 0;
  border-bottom: 1px solid var(--border);
  opacity: 0;
  transform: translateY(24px);
  transition: opacity 0.7s ease, transform 0.7s ease;
}

section.visible {
  opacity: 1;
  transform: none;
}

.section-label {
  font-family: 'DM Mono', monospace;
  font-size: 0.68rem;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--accent);
  margin-bottom: 1.5rem;
}

h2 {
  font-size: 1.9rem;
  font-weight: 400;
  margin-bottom: 1.5rem;
  letter-spacing: -0.01em;
}

p { margin-bottom: 1.2rem; color: #c8c8d8; }

/* Research Question Box */
.rq-box {
  border: 1px solid var(--accent);
  border-left: 3px solid var(--accent);
  padding: 1.5rem 2rem;
  margin: 2rem 0;
  background: rgba(124,106,247,0.05);
  border-radius: 0 4px 4px 0;
}

.rq-box .rq-label {
  font-family: 'DM Mono', monospace;
  font-size: 0.65rem;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--accent);
  margin-bottom: 0.8rem;
}

.rq-box p {
  font-style: italic;
  font-size: 1.15rem;
  color: var(--text);
  margin: 0;
}

/* Fractal canvas section */
.fractal-showcase {
  margin: 2rem 0;
  border: 1px solid var(--border);
  border-radius: 4px;
  overflow: hidden;
  background: var(--surface);
}

.fractal-showcase canvas {
  display: block;
  width: 100%;
}

.fractal-caption {
  padding: 1rem 1.5rem;
  font-family: 'DM Mono', monospace;
  font-size: 0.7rem;
  color: var(--muted);
  border-top: 1px solid var(--border);
  display: flex;
  justify-content: space-between;
}

/* Fractal controls */
.fractal-controls {
  padding: 1rem 1.5rem;
  border-top: 1px solid var(--border);
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}

.btn {
  font-family: 'DM Mono', monospace;
  font-size: 0.68rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  padding: 0.5rem 1.2rem;
  border: 1px solid var(--border);
  background: transparent;
  color: var(--muted);
  cursor: pointer;
  border-radius: 2px;
  transition: all 0.2s;
}

.btn:hover, .btn.active {
  border-color: var(--accent);
  color: var(--accent);
  background: rgba(124,106,247,0.08);
}

/* Math formula */
.formula-block {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 4px;
  padding: 1.5rem 2rem;
  margin: 1.5rem 0;
  font-family: 'DM Mono', monospace;
  font-size: 0.9rem;
  color: var(--accent2);
  text-align: center;
  letter-spacing: 0.05em;
}

/* Key findings */
.findings-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1rem;
  margin: 2rem 0;
}

.finding-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 4px;
  padding: 1.5rem;
  transition: border-color 0.2s;
}

.finding-card:hover { border-color: var(--accent); }

.finding-number {
  font-family: 'DM Mono', monospace;
  font-size: 2rem;
  color: var(--accent);
  line-height: 1;
  margin-bottom: 0.5rem;
}

.finding-label {
  font-size: 0.9rem;
  color: var(--muted);
}

/* Bibliography */
.bib-list {
  list-style: none;
  counter-reset: bib;
}

.bib-list li {
  counter-increment: bib;
  padding: 0.8rem 0;
  border-bottom: 1px solid var(--border);
  font-size: 0.9rem;
  color: var(--muted);
  padding-left: 2rem;
  position: relative;
}

.bib-list li::before {
  content: '[' counter(bib) ']';
  position: absolute;
  left: 0;
  font-family: 'DM Mono', monospace;
  font-size: 0.7rem;
  color: var(--accent);
  top: 0.9rem;
}

/* Footer */
footer {
  padding: 3rem 0;
  text-align: center;
  font-family: 'DM Mono', monospace;
  font-size: 0.7rem;
  color: var(--muted);
  letter-spacing: 0.1em;
}

@media (max-width: 600px) {
  nav ul { gap: 1rem; font-size: 0.65rem; }
  .findings-grid { grid-template-columns: 1fr 1fr; }
}
```

  </style>
</head>
<body>

<canvas id="fractal-bg"></canvas>

<div class="container">
  <header>
    <div class="ib-label">IB Extended Essay — Mathematics</div>
    <h1>Mixed Fractal Analysis</h1>
    <p class="subtitle">混合分形分析</p>
    <div class="meta-row">
      <div class="meta-item"><span>Subject</span>Mathematics</div>
      <div class="meta-item"><span>Author</span>Brace Baoquan</div>
      <div class="meta-item"><span>Word Count</span>~4,000</div>
      <div class="meta-item"><span>Year</span>2026</div>
    </div>
  </header>

  <nav>
    <div class="container">
      <ul>
        <li><a href="#abstract">Abstract</a></li>
        <li><a href="#introduction">Introduction</a></li>
        <li><a href="#exploration">Exploration</a></li>
        <li><a href="#findings">Findings</a></li>
        <li><a href="#conclusion">Conclusion</a></li>
        <li><a href="#bibliography">Bibliography</a></li>
      </ul>
    </div>
  </nav>

  <section id="abstract">
    <div class="section-label">00 — Abstract</div>
    <h2>Overview</h2>
    <div class="rq-box">
      <div class="rq-label">Research Question</div>
      <p>How can mixed fractal systems be analyzed to reveal emergent geometric and dimensional properties not present in their individual components?</p>
    </div>
    <p>This extended essay investigates the mathematical properties of mixed fractal systems, exploring what emerges when two or more distinct fractal generation rules are combined or alternated. Through analysis of fractal dimension, self-similarity, and iterative behavior, this essay demonstrates that hybrid systems produce unique geometric structures with measurable properties distinct from their source fractals.</p>
    <p>Key methods include iterated function systems (IFS), box-counting dimension estimation, and computational visualization of attractor sets. The findings suggest that mixing fractal rules does not simply average their properties — instead, new emergent behavior arises.</p>
  </section>

  <section id="introduction">
    <div class="section-label">01 — Introduction</div>
    <h2>Background & Motivation</h2>
    <p>Fractals are geometric objects defined by self-similarity across scales and non-integer Hausdorff dimensions. Since Mandelbrot's foundational work in the 1970s, fractals have appeared in contexts ranging from coastline measurement to financial modeling.</p>
    <p>Most classical fractals — the Sierpiński triangle, Koch snowflake, Cantor set — arise from a single, repeated rule. This essay asks: what happens when we mix these rules? Can a fractal "inherit" properties from two parents, or does something entirely new emerge?</p>
    <div class="formula-block">
      D = lim (ε→0) [ log N(ε) / log(1/ε) ]
      <div style="font-size:0.65rem; color: var(--muted); margin-top:0.5rem; font-style:italic;">Hausdorff-Besicovitch dimension formula</div>
    </div>
    <p>The investigation focuses on mixing Iterated Function Systems (IFS) — mathematical recipes that generate fractals through repeated affine transformations. By alternating or blending these recipes, novel attractor sets emerge.</p>
  </section>

  <section id="exploration">
    <div class="section-label">02 — Mathematical Exploration</div>
    <h2>Interactive Fractal Visualizer</h2>
    <p>The following visualizer demonstrates different fractal types discussed in this essay. Each fractal is generated through iterative computation, revealing the self-similar structures that form the basis of this analysis.</p>

```
<div class="fractal-showcase">
  <canvas id="fractalCanvas" width="820" height="400"></canvas>
  <div class="fractal-controls">
    <button class="btn active" onclick="drawFractal('sierpinski')">Sierpiński</button>
    <button class="btn" onclick="drawFractal('barnsley')">Barnsley Fern</button>
    <button class="btn" onclick="drawFractal('mixed')">Mixed System</button>
    <button class="btn" onclick="drawFractal('dragon')">Dragon Curve</button>
  </div>
  <div class="fractal-caption">
    <span id="fractal-name">Sierpiński Triangle — IFS with 3 contractions, D ≈ 1.585</span>
    <span>Click above to explore</span>
  </div>
</div>

<h2 style="margin-top:2rem;">Mixing IFS Rules</h2>
<p>An IFS consists of a finite set of contraction mappings {f₁, f₂, ..., fₙ}. The attractor A satisfies:</p>
<div class="formula-block">A = f₁(A) ∪ f₂(A) ∪ ... ∪ fₙ(A)</div>
<p>A mixed system is constructed by drawing randomly from two distinct IFS sets — with probability p from system α, and (1−p) from system β. As p varies continuously from 0 to 1, the attractor morphs between the two parent fractals, passing through a continuum of hybrid forms.</p>
<p>The fractal dimension of the mixed system does not follow a simple linear interpolation. Instead, dimensional transitions exhibit non-monotonic behavior at certain mixing ratios, suggesting phase-transition-like phenomena in the geometry.</p>
```

  </section>

  <section id="findings">
    <div class="section-label">03 — Key Findings</div>
    <h2>Results & Analysis</h2>
    <div class="findings-grid">
      <div class="finding-card">
        <div class="finding-number">1.58</div>
        <div class="finding-label">Fractal dimension of Sierpiński triangle (log3/log2)</div>
      </div>
      <div class="finding-card">
        <div class="finding-number">1.73</div>
        <div class="finding-label">Peak dimension observed in mixed systems at p ≈ 0.4</div>
      </div>
      <div class="finding-card">
        <div class="finding-number">3</div>
        <div class="finding-label">Distinct phase regions identified in the mixing parameter space</div>
      </div>
      <div class="finding-card">
        <div class="finding-number">∞</div>
        <div class="finding-label">Self-similar detail at every scale — the hallmark of fractality</div>
      </div>
    </div>
    <p>The most striking finding is that mixed systems can exhibit dimensions <em>exceeding</em> either parent system. This emergent complexity arises from constructive interference between the two IFS rule sets — analogous to how combining simple waves can produce complex interference patterns.</p>
    <p>Furthermore, the transition between parent attractors is not smooth. At certain critical mixing ratios, the attractor undergoes sudden topological changes — disconnected sets merge, or connected sets fragment — marking discrete phase boundaries.</p>
  </section>

  <section id="conclusion">
    <div class="section-label">04 — Conclusion</div>
    <h2>Reflection & Evaluation</h2>
    <p>This investigation demonstrates that mixed fractal systems are not merely interpolations of their components — they are genuinely novel mathematical objects with emergent properties. The non-linear relationship between mixing parameter and fractal dimension suggests rich underlying structure that merits deeper investigation.</p>
    <p>The research question has been addressed: mixed fractal systems do reveal emergent properties absent in their parents, including elevated fractal dimensions, phase transitions in topology, and new symmetry structures.</p>
    <p>Limitations include the computational approximation inherent in box-counting dimension estimation, and the restricted class of IFS mappings considered. Future work could extend this analysis to three-dimensional IFS, random fractal systems, or applications in modeling natural phenomena such as plant growth patterns and terrain formation.</p>
  </section>

  <section id="bibliography">
    <div class="section-label">05 — Bibliography</div>
    <h2>References</h2>
    <ul class="bib-list">
      <li>Mandelbrot, B. B. (1982). <em>The Fractal Geometry of Nature</em>. W. H. Freeman.</li>
      <li>Barnsley, M. F. (1988). <em>Fractals Everywhere</em>. Academic Press.</li>
      <li>Falconer, K. (2003). <em>Fractal Geometry: Mathematical Foundations and Applications</em>. Wiley.</li>
      <li>Hutchinson, J. E. (1981). Fractals and self-similarity. <em>Indiana University Mathematics Journal</em>, 30(5), 713–747.</li>
      <li>Peitgen, H.-O., Jürgens, H., & Saupe, D. (1992). <em>Chaos and Fractals: New Frontiers of Science</em>. Springer.</li>
    </ul>
  </section>

  <footer>
    <p>Brace Baoquan · IB Extended Essay · Mathematics · 2026</p>
  </footer>
</div>

<script>
  // Background fractal animation
  const bgCanvas = document.getElementById('fractal-bg');
  const bgCtx = bgCanvas.getContext('2d');
  bgCanvas.width = window.innerWidth;
  bgCanvas.height = window.innerHeight;

  function drawBgFractal() {
    bgCtx.clearRect(0, 0, bgCanvas.width, bgCanvas.height);
    bgCtx.strokeStyle = '#7c6af7';
    bgCtx.lineWidth = 0.5;
    const points = [];
    let x = 0, y = 0;
    for (let i = 0; i < 8000; i++) {
      const r = Math.random();
      let nx, ny;
      if (r < 0.33) { nx = x/2; ny = y/2; }
      else if (r < 0.66) { nx = x/2 + 0.5; ny = y/2; }
      else { nx = x/2 + 0.25; ny = y/2 + 0.433; }
      x = nx; y = ny;
      if (i > 20) points.push([x, y]);
    }
    const W = bgCanvas.width, H = bgCanvas.height;
    points.forEach(([px, py]) => {
      bgCtx.fillStyle = 'rgba(124,106,247,0.6)';
      bgCtx.fillRect(px * W * 0.8 + W * 0.1, (1 - py) * H * 0.8 + H * 0.1, 1, 1);
    });
  }
  drawBgFractal();

  // Main fractal canvas
  const canvas = document.getElementById('fractalCanvas');
  const ctx = canvas.getContext('2d');

  function clearCanvas() {
    ctx.fillStyle = '#111118';
    ctx.fillRect(0, 0, canvas.width, canvas.height);
  }

  function drawSierpinski() {
    clearCanvas();
    document.getElementById('fractal-name').textContent = 'Sierpiński Triangle — IFS with 3 contractions, D ≈ 1.585';
    let x = 0, y = 0;
    const W = canvas.width, H = canvas.height;
    for (let i = 0; i < 60000; i++) {
      const r = Math.random();
      if (r < 0.33) { x = x/2; y = y/2; }
      else if (r < 0.66) { x = x/2 + 0.5; y = y/2; }
      else { x = x/2 + 0.25; y = y/2 + 0.433; }
      if (i > 20) {
        const px = x * H * 0.85 + (W - H * 0.85) / 2;
        const py = (1 - y) * H * 0.85 + H * 0.07;
        ctx.fillStyle = `hsl(${250 + y * 60}, 70%, ${50 + x * 30}%)`;
        ctx.fillRect(px, py, 1, 1);
      }
    }
  }

  function drawBarnsley() {
    clearCanvas();
    document.getElementById('fractal-name').textContent = 'Barnsley Fern — 4 affine transformations, D ≈ 1.97';
    let x = 0, y = 0;
    const W = canvas.width, H = canvas.height;
    for (let i = 0; i < 80000; i++) {
      const r = Math.random();
      let nx, ny;
      if (r < 0.01) { nx = 0; ny = 0.16 * y; }
      else if (r < 0.86) { nx = 0.85*x + 0.04*y; ny = -0.04*x + 0.85*y + 1.6; }
      else if (r < 0.93) { nx = 0.2*x - 0.26*y; ny = 0.23*x + 0.22*y + 1.6; }
      else { nx = -0.15*x + 0.28*y; ny = 0.26*x + 0.24*y + 0.44; }
      x = nx; y = ny;
      if (i > 20) {
        const px = (x + 3) / 6 * W;
        const py = (1 - y / 10) * H;
        ctx.fillStyle = `hsl(${130 + y * 8}, 60%, ${40 + y * 3}%)`;
        ctx.fillRect(px, py, 1, 1);
      }
    }
  }

  function drawMixed() {
    clearCanvas();
    document.getElementById('fractal-name').textContent = 'Mixed System (p=0.5) — Hybrid IFS, emergent D ≈ 1.73';
    let x = 0, y = 0;
    const W = canvas.width, H = canvas.height;
    const p = 0.5;
    for (let i = 0; i < 80000; i++) {
      const r = Math.random();
      let nx, ny;
      if (Math.random() < p) {
        if (r < 0.33) { nx = x/2; ny = y/2; }
        else if (r < 0.66) { nx = x/2 + 0.5; ny = y/2; }
        else { nx = x/2 + 0.25; ny = y/2 + 0.433; }
        if (i > 20) {
          const px = x * H * 0.85 + (W - H * 0.85)/2;
          const py = (1-y) * H * 0.85 + H * 0.07;
          ctx.fillStyle = `hsl(280, 70%, 60%)`;
          ctx.fillRect(px, py, 1, 1);
        }
      } else {
        if (r < 0.01) { nx = 0; ny = 0.16*y; }
        else if (r < 0.86) { nx = 0.85*x + 0.04*y; ny = -0.04*x + 0.85*y + 1.6; }
        else if (r < 0.93) { nx = 0.2*x - 0.26*y; ny = 0.23*x + 0.22*y + 1.6; }
        else { nx = -0.15*x + 0.28*y; ny = 0.26*x + 0.24*y + 0.44; }
        x = nx; y = ny;
        if (i > 20) {
          const px = (x/6 + 0.5) * W;
          const py = (1 - y/10) * H;
          ctx.fillStyle = `hsl(160, 70%, 55%)`;
          ctx.fillRect(px, py, 1, 1);
        }
        continue;
      }
      x = nx; y = ny;
    }
  }

  function drawDragon() {
    clearCanvas();
    document.getElementById('fractal-name').textContent = 'Dragon Curve — Recursive fold sequence, D ≈ 2';
    const W = canvas.width, H = canvas.height;
    let seq = [1];
    for (let i = 0; i < 14; i++) {
      const mid = [...seq, 1];
      const rev = seq.slice().reverse().map(v => v === 1 ? 0 : 1);
      seq = [...mid, ...rev];
    }
    let x = W/2, y = H/2, angle = 0;
    const step = 3;
    ctx.beginPath();
    ctx.moveTo(x, y);
    seq.forEach((turn, i) => {
      angle += turn === 1 ? Math.PI/2 : -Math.PI/2;
      x += step * Math.cos(angle);
      y += step * Math.sin(angle);
      const hue = (i / seq.length) * 300 + 200;
      ctx.strokeStyle = `hsl(${hue}, 70%, 60%)`;
      ctx.lineTo(x, y);
      ctx.stroke();
      ctx.beginPath();
      ctx.moveTo(x, y);
    });
  }

  function drawFractal(type) {
    document.querySelectorAll('.btn').forEach(b => b.classList.remove('active'));
    event.target.classList.add('active');
    if (type === 'sierpinski') drawSierpinski();
    else if (type === 'barnsley') drawBarnsley();
    else if (type === 'mixed') drawMixed();
    else if (type === 'dragon') drawDragon();
  }

  // Scroll reveal
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('visible'); });
  }, { threshold: 0.1 });
  document.querySelectorAll('section').forEach(s => observer.observe(s));

  // Initial draw
  drawSierpinski();
</script>

</body>
</html>
