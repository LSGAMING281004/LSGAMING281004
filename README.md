## Hi there 👋

<!--
**LSGAMING281004/LSGAMING281004** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>LOKESH K — Full Stack Java Developer</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@300;400;500;700&family=Syne:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --green: #00ff88;
    --cyan: #00d4ff;
    --purple: #bf5fff;
    --amber: #ffb830;
    --bg0: #060810;
    --bg1: #0c1018;
    --bg2: #111620;
    --bg3: #181e2c;
    --border: rgba(0,255,136,0.15);
    --border2: rgba(0,212,255,0.15);
    --text: #e2e8f0;
    --muted: #64748b;
    --font-mono: 'JetBrains Mono', monospace;
    --font-display: 'Syne', sans-serif;
  }

  html { scroll-behavior: smooth; }

  body {
    background: var(--bg0);
    color: var(--text);
    font-family: var(--font-mono);
    min-height: 100vh;
    overflow-x: hidden;
    position: relative;
  }

  /* Grid background */
  body::before {
    content: '';
    position: fixed;
    inset: 0;
    background-image:
      linear-gradient(rgba(0,255,136,0.03) 1px, transparent 1px),
      linear-gradient(90deg, rgba(0,255,136,0.03) 1px, transparent 1px);
    background-size: 40px 40px;
    pointer-events: none;
    z-index: 0;
  }

  /* Radial glow */
  body::after {
    content: '';
    position: fixed;
    top: -20%;
    left: -10%;
    width: 60%;
    height: 60%;
    background: radial-gradient(ellipse, rgba(0,255,136,0.06) 0%, transparent 70%);
    pointer-events: none;
    z-index: 0;
  }

  .container {
    max-width: 900px;
    margin: 0 auto;
    padding: 2rem 1.5rem 4rem;
    position: relative;
    z-index: 1;
  }

  /* ─── TOP BAR ─── */
  .topbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 3rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid var(--border);
  }
  .topbar-left {
    display: flex;
    align-items: center;
    gap: 8px;
    font-size: 12px;
    color: var(--muted);
  }
  .dot { width: 10px; height: 10px; border-radius: 50%; }
  .dot.red { background: #ff5f57; }
  .dot.yellow { background: #ffbd2e; }
  .dot.green { background: #28c840; }
  .topbar-cmd {
    font-size: 12px;
    color: var(--green);
    opacity: 0.7;
  }

  /* ─── HERO ─── */
  .hero {
    display: grid;
    grid-template-columns: auto 1fr;
    gap: 2.5rem;
    align-items: start;
    margin-bottom: 2.5rem;
    padding: 2rem;
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 16px;
    position: relative;
    overflow: hidden;
  }
  .hero::before {
    content: '';
    position: absolute;
    top: -60px; right: -60px;
    width: 200px; height: 200px;
    background: radial-gradient(circle, rgba(0,212,255,0.08) 0%, transparent 70%);
    pointer-events: none;
  }

  .avatar-wrapper {
    position: relative;
    flex-shrink: 0;
  }
  .avatar-ring {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    padding: 3px;
    background: linear-gradient(135deg, var(--green), var(--cyan), var(--purple));
    animation: spin-slow 8s linear infinite;
  }
  @keyframes spin-slow {
    from { filter: hue-rotate(0deg); }
    to { filter: hue-rotate(360deg); }
  }
  .avatar-inner {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    overflow: hidden;
    border: 3px solid var(--bg1);
  }
  .avatar-inner img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }
  .status-badge {
    position: absolute;
    bottom: 4px; right: 4px;
    width: 22px; height: 22px;
    border-radius: 50%;
    background: #28c840;
    border: 3px solid var(--bg1);
    box-shadow: 0 0 10px #28c840;
  }

  .hero-info { min-width: 0; }
  .hero-tag {
    font-size: 11px;
    color: var(--green);
    letter-spacing: 3px;
    text-transform: uppercase;
    margin-bottom: 8px;
    opacity: 0.8;
  }
  .hero-name {
    font-family: var(--font-display);
    font-size: 2.6rem;
    font-weight: 800;
    line-height: 1.1;
    letter-spacing: -0.02em;
    background: linear-gradient(120deg, #fff 30%, var(--cyan) 70%, var(--green) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 6px;
  }
  .hero-title {
    font-size: 14px;
    color: var(--cyan);
    margin-bottom: 16px;
    font-weight: 300;
    letter-spacing: 0.5px;
  }
  .hero-bio {
    font-size: 13px;
    color: var(--muted);
    line-height: 1.8;
    margin-bottom: 20px;
    max-width: 520px;
  }

  .meta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    font-size: 12px;
    color: var(--muted);
  }
  .meta-item {
    display: flex;
    align-items: center;
    gap: 6px;
  }
  .meta-item svg { opacity: 0.5; flex-shrink: 0; }

  /* ─── STATS ─── */
  .stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 12px;
    margin-bottom: 2rem;
  }
  .stat-card {
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 1.2rem 1rem;
    text-align: center;
    position: relative;
    overflow: hidden;
    transition: border-color 0.2s, transform 0.2s;
  }
  .stat-card:hover {
    border-color: rgba(0,255,136,0.4);
    transform: translateY(-2px);
  }
  .stat-card::after {
    content: '';
    position: absolute;
    bottom: 0; left: 0; right: 0;
    height: 2px;
    background: var(--green);
    transform: scaleX(0);
    transition: transform 0.3s;
  }
  .stat-card:hover::after { transform: scaleX(1); }
  .stat-num {
    font-family: var(--font-display);
    font-size: 1.9rem;
    font-weight: 800;
    color: var(--green);
    line-height: 1;
    margin-bottom: 6px;
  }
  .stat-label {
    font-size: 10px;
    color: var(--muted);
    letter-spacing: 2px;
    text-transform: uppercase;
  }

  /* ─── SECTION HEADER ─── */
  .section-header {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 1.2rem;
  }
  .section-line {
    height: 1px;
    flex: 1;
    background: var(--border);
  }
  .section-title {
    font-size: 11px;
    color: var(--green);
    letter-spacing: 3px;
    text-transform: uppercase;
    font-weight: 500;
    white-space: nowrap;
  }
  .section-title span { color: var(--muted); }

  /* ─── SKILLS ─── */
  .skills-block {
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 1.5rem;
    margin-bottom: 2rem;
  }
  .skill-group { margin-bottom: 1.2rem; }
  .skill-group:last-child { margin-bottom: 0; }
  .skill-group-label {
    font-size: 10px;
    color: var(--cyan);
    letter-spacing: 2px;
    text-transform: uppercase;
    margin-bottom: 10px;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .skill-group-label::after {
    content: '';
    height: 1px;
    flex: 1;
    background: var(--border2);
  }
  .tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }
  .tag {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 5px 12px;
    border-radius: 6px;
    font-size: 12px;
    font-family: var(--font-mono);
    font-weight: 500;
    transition: all 0.2s;
    cursor: default;
    border: 1px solid;
  }
  .tag:hover { transform: translateY(-1px); }
  .tag.java { background: rgba(244,67,54,0.1); border-color: rgba(244,67,54,0.3); color: #ff8a80; }
  .tag.js { background: rgba(255,184,48,0.1); border-color: rgba(255,184,48,0.3); color: var(--amber); }
  .tag.sql { background: rgba(0,212,255,0.08); border-color: rgba(0,212,255,0.25); color: var(--cyan); }
  .tag.spring { background: rgba(40,200,64,0.08); border-color: rgba(40,200,64,0.25); color: #69db7c; }
  .tag.react { background: rgba(97,218,251,0.08); border-color: rgba(97,218,251,0.25); color: #61dafb; }
  .tag.db { background: rgba(191,95,255,0.08); border-color: rgba(191,95,255,0.25); color: var(--purple); }
  .tag.tool { background: rgba(255,255,255,0.04); border-color: rgba(255,255,255,0.1); color: #94a3b8; }
  .tag.api { background: rgba(0,255,136,0.08); border-color: rgba(0,255,136,0.25); color: var(--green); }

  /* ─── PROJECTS ─── */
  .projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 16px;
    margin-bottom: 2rem;
  }
  .project-card {
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 1.4rem;
    position: relative;
    overflow: hidden;
    transition: all 0.25s;
    display: flex;
    flex-direction: column;
  }
  .project-card:hover {
    border-color: rgba(0,255,136,0.35);
    transform: translateY(-3px);
    box-shadow: 0 12px 40px rgba(0,255,136,0.06);
  }
  .project-card::before {
    content: attr(data-num);
    position: absolute;
    top: 12px; right: 16px;
    font-size: 3rem;
    font-weight: 800;
    font-family: var(--font-display);
    color: rgba(255,255,255,0.03);
    line-height: 1;
    pointer-events: none;
  }

  .proj-header {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    margin-bottom: 10px;
  }
  .proj-icon {
    width: 36px; height: 36px;
    border-radius: 8px;
    display: flex; align-items: center; justify-content: center;
    font-size: 16px;
    margin-right: 10px;
    flex-shrink: 0;
  }
  .icon-blue { background: rgba(0,212,255,0.1); }
  .icon-green { background: rgba(0,255,136,0.1); }
  .icon-purple { background: rgba(191,95,255,0.1); }

  .proj-title {
    font-family: var(--font-display);
    font-size: 15px;
    font-weight: 700;
    color: #fff;
    margin-bottom: 4px;
  }
  .proj-sub {
    font-size: 10px;
    color: var(--muted);
    letter-spacing: 1px;
    text-transform: uppercase;
  }
  .proj-desc {
    font-size: 12px;
    color: var(--muted);
    line-height: 1.7;
    margin-bottom: 14px;
    flex: 1;
  }
  .proj-highlight {
    font-size: 11px;
    color: var(--green);
    margin-bottom: 14px;
    padding: 8px 10px;
    background: rgba(0,255,136,0.04);
    border-left: 2px solid var(--green);
    border-radius: 0 6px 6px 0;
    line-height: 1.6;
  }
  .proj-tags { display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 16px; }
  .ptag {
    font-size: 10px;
    padding: 3px 8px;
    border-radius: 4px;
    border: 1px solid rgba(255,255,255,0.08);
    color: var(--muted);
    font-family: var(--font-mono);
  }
  .proj-links {
    display: flex;
    gap: 8px;
    margin-top: auto;
  }
  .plink {
    display: inline-flex;
    align-items: center;
    gap: 5px;
    font-size: 11px;
    padding: 5px 12px;
    border-radius: 6px;
    text-decoration: none;
    transition: all 0.2s;
    border: 1px solid;
  }
  .plink.demo {
    background: rgba(0,212,255,0.08);
    border-color: rgba(0,212,255,0.25);
    color: var(--cyan);
  }
  .plink.demo:hover { background: rgba(0,212,255,0.15); }
  .plink.gh {
    background: rgba(255,255,255,0.04);
    border-color: rgba(255,255,255,0.1);
    color: var(--muted);
  }
  .plink.gh:hover { color: #fff; border-color: rgba(255,255,255,0.25); }

  /* ─── ACTIVITY / CONTRIB ─── */
  .contrib-block {
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 1.5rem;
    margin-bottom: 2rem;
    overflow: hidden;
  }
  .contrib-grid {
    display: flex;
    gap: 3px;
    flex-wrap: wrap;
    margin-top: 1rem;
  }
  .contrib-week { display: flex; flex-direction: column; gap: 3px; }
  .contrib-cell {
    width: 12px;
    height: 12px;
    border-radius: 2px;
    transition: transform 0.1s;
  }
  .contrib-cell:hover { transform: scale(1.3); }
  .c0 { background: rgba(255,255,255,0.04); }
  .c1 { background: rgba(0,255,136,0.15); }
  .c2 { background: rgba(0,255,136,0.35); }
  .c3 { background: rgba(0,255,136,0.6); }
  .c4 { background: rgba(0,255,136,0.9); }

  /* ─── CERTIFICATIONS ─── */
  .cert-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 12px;
    margin-bottom: 2rem;
  }
  .cert-card {
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 1.2rem;
    display: flex;
    align-items: center;
    gap: 14px;
    transition: all 0.2s;
  }
  .cert-card:hover {
    border-color: rgba(0,212,255,0.3);
    transform: translateY(-1px);
  }
  .cert-icon {
    width: 40px; height: 40px;
    border-radius: 10px;
    display: flex; align-items: center; justify-content: center;
    font-size: 18px;
    flex-shrink: 0;
  }
  .ci-java { background: rgba(244,67,54,0.12); }
  .ci-ibm { background: rgba(0,212,255,0.1); }
  .ci-hr { background: rgba(0,255,136,0.1); }
  .cert-name {
    font-size: 13px;
    font-weight: 500;
    color: var(--text);
    margin-bottom: 3px;
  }
  .cert-by {
    font-size: 11px;
    color: var(--muted);
  }
  .cert-year {
    margin-left: auto;
    font-size: 11px;
    color: var(--cyan);
    flex-shrink: 0;
  }

  /* ─── ACHIEVEMENTS ─── */
  .ach-row {
    display: flex;
    gap: 12px;
    flex-wrap: wrap;
    margin-bottom: 2rem;
  }
  .ach-badge {
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 10px 16px;
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 10px;
    font-size: 12px;
    color: var(--text);
    transition: all 0.2s;
  }
  .ach-badge:hover {
    border-color: rgba(255,184,48,0.4);
    color: var(--amber);
  }
  .ach-badge svg { color: var(--amber); }
  .ach-sub { font-size: 10px; color: var(--muted); display: block; }

  /* ─── EDUCATION ─── */
  .edu-card {
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 1.4rem;
    display: flex;
    gap: 16px;
    align-items: flex-start;
    margin-bottom: 2rem;
    transition: border-color 0.2s;
  }
  .edu-card:hover { border-color: rgba(191,95,255,0.3); }
  .edu-dot {
    width: 44px; height: 44px;
    border-radius: 12px;
    background: rgba(191,95,255,0.1);
    border: 1px solid rgba(191,95,255,0.25);
    display: flex; align-items: center; justify-content: center;
    font-size: 20px;
    flex-shrink: 0;
  }
  .edu-degree {
    font-family: var(--font-display);
    font-size: 16px;
    font-weight: 700;
    color: #fff;
    margin-bottom: 4px;
  }
  .edu-inst {
    font-size: 13px;
    color: var(--purple);
    margin-bottom: 8px;
  }
  .edu-meta {
    display: flex;
    gap: 16px;
    font-size: 12px;
    color: var(--muted);
  }
  .edu-score {
    margin-left: auto;
    font-size: 22px;
    font-family: var(--font-display);
    font-weight: 800;
    color: var(--green);
    flex-shrink: 0;
    text-align: right;
  }
  .edu-score span { display: block; font-size: 10px; color: var(--muted); font-family: var(--font-mono); text-align: right; }

  /* ─── CONTACT / SOCIAL ─── */
  .social-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
    gap: 10px;
    margin-bottom: 2rem;
  }
  .social-link {
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 12px 14px;
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 10px;
    text-decoration: none;
    transition: all 0.2s;
    color: var(--muted);
    font-size: 12px;
  }
  .social-link:hover {
    color: var(--text);
    transform: translateY(-2px);
  }
  .social-link.gh-link:hover { border-color: rgba(255,255,255,0.3); }
  .social-link.li-link:hover { border-color: rgba(0,119,181,0.6); color: #0077b5; }
  .social-link.lc-link:hover { border-color: rgba(255,184,48,0.5); color: var(--amber); }
  .social-link.ig-link:hover { border-color: rgba(228,64,95,0.5); color: #e4405f; }
  .social-link.em-link:hover { border-color: rgba(0,212,255,0.4); color: var(--cyan); }
  .social-link.pf-link:hover { border-color: rgba(0,255,136,0.4); color: var(--green); }
  .social-handle { font-size: 11px; color: var(--muted); }

  /* ─── FOOTER ─── */
  .footer {
    text-align: center;
    padding-top: 2rem;
    border-top: 1px solid var(--border);
    font-size: 11px;
    color: var(--muted);
    letter-spacing: 2px;
  }
  .footer strong { color: var(--green); }

  /* ─── TYPING CURSOR ─── */
  .cursor {
    display: inline-block;
    width: 2px;
    height: 1em;
    background: var(--green);
    animation: blink 1s step-end infinite;
    vertical-align: text-bottom;
  }
  @keyframes blink {
    50% { opacity: 0; }
  }

  /* ─── PINNED REPOS ─── */
  .pinned-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 10px;
    margin-bottom: 2rem;
  }
  .pinned-card {
    background: var(--bg1);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 1rem 1.1rem;
    transition: all 0.2s;
    text-decoration: none;
    display: block;
  }
  .pinned-card:hover {
    border-color: rgba(0,255,136,0.3);
    transform: translateY(-2px);
  }
  .pinned-name {
    font-size: 13px;
    font-weight: 500;
    color: var(--cyan);
    margin-bottom: 5px;
    display: flex;
    align-items: center;
    gap: 6px;
  }
  .pinned-desc {
    font-size: 11px;
    color: var(--muted);
    line-height: 1.6;
    margin-bottom: 10px;
  }
  .pinned-foot {
    display: flex;
    align-items: center;
    gap: 12px;
    font-size: 11px;
    color: var(--muted);
  }
  .lang-dot {
    width: 10px; height: 10px;
    border-radius: 50%;
    flex-shrink: 0;
  }
  .lang-java { background: #b07219; }
  .lang-js { background: #f1e05a; }

  /* ─── ENTRANCE ANIMATIONS ─── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(16px); }
    to { opacity: 1; transform: translateY(0); }
  }
  .hero { animation: fadeUp 0.5s ease both 0.1s; }
  .stats-grid { animation: fadeUp 0.5s ease both 0.2s; }
  .skills-block { animation: fadeUp 0.5s ease both 0.3s; }
  .projects-grid { animation: fadeUp 0.5s ease both 0.4s; }

  @media (max-width: 640px) {
    .hero { grid-template-columns: 1fr; }
    .stats-grid { grid-template-columns: repeat(2, 1fr); }
    .hero-name { font-size: 2rem; }
    .avatar-ring { width: 80px; height: 80px; }
  }
</style>
</head>
<body>
<div class="container">

  <!-- TOP BAR -->
  <div class="topbar">
    <div class="topbar-left">
      <div class="dot red"></div>
      <div class="dot yellow"></div>
      <div class="dot green"></div>
    </div>
    <div class="topbar-cmd">~/lokesh-k <span style="color:var(--muted)">$</span> cat profile.json<span class="cursor"></span></div>
    <div style="font-size:11px;color:var(--muted)">v2025.1</div>
  </div>

  <!-- HERO -->
  <div class="hero">
    <div class="avatar-wrapper">
      <div class="avatar-ring">
        <div class="avatar-inner">
          <img src="https://avatars.githubusercontent.com/u/135082681?v=4" alt="Lokesh K" />
        </div>
      </div>
      <div class="status-badge"></div>
    </div>
    <div class="hero-info">
      <div class="hero-tag">// full stack developer</div>
      <div class="hero-name">LOKESH K</div>
      <div class="hero-title">Spring Boot &nbsp;|&nbsp; React.js &nbsp;|&nbsp; Java &nbsp;|&nbsp; MySQL</div>
      <p class="hero-bio">
        Passionate Full-Stack Developer building robust, scalable backend systems and modern web applications.
        Experienced with RESTful APIs, authentication systems, and cloud-ready architectures. Always exploring
        AI &amp; ML to craft intelligent solutions.
      </p>
      <div class="meta-row">
        <div class="meta-item">
          <svg width="13" height="13" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>
          Cheyyar, Tamil Nadu
        </div>
        <div class="meta-item">
          <svg width="13" height="13" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M21 16V8a2 2 0 00-1-1.73l-7-4a2 2 0 00-2 0l-7 4A2 2 0 003 8v8a2 2 0 001 1.73l7 4a2 2 0 002 0l7-4A2 2 0 0021 16z"/></svg>
          @BerrybeansTech
        </div>
        <div class="meta-item">
          <svg width="13" height="13" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M2 9h20"/></svg>
          lsgaming342@gmail.com
        </div>
        <div class="meta-item">
          <svg width="13" height="13" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07A19.5 19.5 0 013.07 8.81a19.79 19.79 0 01-3.07-8.66A2 2 0 012 0h3a2 2 0 012 1.72c.127.96.361 1.903.7 2.81a2 2 0 01-.45 2.11L6.09 7.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0122 14.92z"/></svg>
          +91 72007 50342
        </div>
      </div>
    </div>
  </div>

  <!-- STATS -->
  <div class="stats-grid">
    <div class="stat-card">
      <div class="stat-num">31</div>
      <div class="stat-label">Repositories</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">15+</div>
      <div class="stat-label">APIs Built</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">3</div>
      <div class="stat-label">Certifications</div>
    </div>
    <div class="stat-card">
      <div class="stat-num" style="color:var(--cyan)">72%</div>
      <div class="stat-label">BCA Score</div>
    </div>
  </div>

  <!-- SKILLS -->
  <div class="section-header">
    <div class="section-title"><span>01.</span> tech stack</div>
    <div class="section-line"></div>
  </div>
  <div class="skills-block">
    <div class="skill-group">
      <div class="skill-group-label">Languages</div>
      <div class="tags">
        <span class="tag java">☕ Java</span>
        <span class="tag js">⚡ JavaScript</span>
        <span class="tag sql">🔷 SQL</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-label">Backend &amp; API</div>
      <div class="tags">
        <span class="tag spring">🍃 Spring Boot</span>
        <span class="tag api">⚙ REST API</span>
        <span class="tag api">🔐 Auth Systems</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-label">Frontend</div>
      <div class="tags">
        <span class="tag react">⚛ React.js</span>
        <span class="tag js">📄 HTML5</span>
        <span class="tag js">🎨 CSS3</span>
        <span class="tag tool">📐 Bootstrap</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-label">Database</div>
      <div class="tags">
        <span class="tag db">🐬 MySQL</span>
        <span class="tag db">🐘 PostgreSQL</span>
        <span class="tag db">🔥 Firebase</span>
      </div>
    </div>
    <div class="skill-group">
      <div class="skill-group-label">Tools &amp; Platform</div>
      <div class="tags">
        <span class="tag tool">🔧 Git</span>
        <span class="tag tool">🐙 GitHub</span>
        <span class="tag tool">📝 VS Code</span>
        <span class="tag db">🔥 Firebase</span>
        <span class="tag tool">📱 Android</span>
      </div>
    </div>
  </div>

  <!-- FEATURED PROJECTS -->
  <div class="section-header">
    <div class="section-title"><span>02.</span> featured projects</div>
    <div class="section-line"></div>
  </div>
  <div class="projects-grid">
    <!-- ShoppinGo -->
    <div class="project-card" data-num="01">
      <div class="proj-header">
        <div style="display:flex;align-items:center;gap:10px">
          <div class="proj-icon icon-blue">🛍</div>
          <div>
            <div class="proj-title">ShoppinGo</div>
            <div class="proj-sub">Store Discovery Platform</div>
          </div>
        </div>
      </div>
      <p class="proj-desc">Full-stack platform serving multi-role users — public &amp; store owners — with comprehensive store management and review system.</p>
      <div class="proj-highlight">⚡ Built 15+ RESTful APIs · Optimized DB queries by ~30% · Role-based auth</div>
      <div class="proj-tags">
        <span class="ptag">Spring Boot</span>
        <span class="ptag">React.js</span>
        <span class="ptag">MySQL</span>
        <span class="ptag">REST API</span>
      </div>
      <div class="proj-links">
        <a href="https://shoppingo-acb4f.web.app/" class="plink demo" target="_blank">↗ Live Demo</a>
        <a href="https://github.com/LSGAMING281004/ShoppinGo" class="plink gh" target="_blank">{ } GitHub</a>
      </div>
    </div>

    <!-- Notemee -->
    <div class="project-card" data-num="02">
      <div class="proj-header">
        <div style="display:flex;align-items:center;gap:10px">
          <div class="proj-icon icon-green">📒</div>
          <div>
            <div class="proj-title">Notemee</div>
            <div class="proj-sub">Secure Note Management</div>
          </div>
        </div>
      </div>
      <p class="proj-desc">Responsive note-taking web app enabling users to save and manage daily thoughts securely with Google authentication.</p>
      <div class="proj-highlight">🔒 Google Auth SSO · Optimised state handling · Minimal UX design</div>
      <div class="proj-tags">
        <span class="ptag">React.js</span>
        <span class="ptag">Firebase</span>
        <span class="ptag">Google Auth</span>
        <span class="ptag">Responsive</span>
      </div>
      <div class="proj-links">
        <a href="https://account-create-2c8fb.web.app" class="plink demo" target="_blank">↗ Live Demo</a>
        <a href="https://github.com/LSGAMING281004/Notemee" class="plink gh" target="_blank">{ } GitHub</a>
      </div>
    </div>

    <!-- Jarvis -->
    <div class="project-card" data-num="03">
      <div class="proj-header">
        <div style="display:flex;align-items:center;gap:10px">
          <div class="proj-icon icon-purple">🤖</div>
          <div>
            <div class="proj-title">Jarvis</div>
            <div class="proj-sub">Android AI Assistant</div>
          </div>
        </div>
      </div>
      <p class="proj-desc">Intelligent Android-based voice assistant with speech recognition and intent processing capabilities — final year project.</p>
      <div class="proj-highlight">🎙 Voice commands · Auto-calling &amp; SMS workflows · Modular architecture</div>
      <div class="proj-tags">
        <span class="ptag">Android</span>
        <span class="ptag">Firebase ML Kit</span>
        <span class="ptag">Java</span>
        <span class="ptag">Voice Recognition</span>
      </div>
      <div class="proj-links">
        <a href="https://github.com/LSGAMING281004/Jarvis" class="plink demo" target="_blank">↗ View Project</a>
        <a href="https://github.com/LSGAMING281004/Jarvis" class="plink gh" target="_blank">{ } GitHub</a>
      </div>
    </div>
  </div>

  <!-- PINNED REPOS -->
  <div class="section-header">
    <div class="section-title"><span>03.</span> pinned repos</div>
    <div class="section-line"></div>
  </div>
  <div class="pinned-grid" style="margin-bottom:2rem;">
    <a class="pinned-card" href="https://github.com/LSGAMING281004/Java-Programs" target="_blank">
      <div class="pinned-name">
        <svg width="14" height="14" fill="none" stroke="var(--cyan)" stroke-width="2" viewBox="0 0 24 24"><path d="M3 3h18v18H3z"/><path d="M3 9h18M9 21V9"/></svg>
        Java-Programs
      </div>
      <div class="pinned-desc">Java problems and logic file — practice &amp; algorithm challenges</div>
      <div class="pinned-foot">
        <div class="lang-dot lang-java"></div> Java
        <span>⭐ 1</span>
      </div>
    </a>
    <a class="pinned-card" href="https://github.com/LSGAMING281004/React.js-mini-projects-" target="_blank">
      <div class="pinned-name">
        <svg width="14" height="14" fill="none" stroke="var(--cyan)" stroke-width="2" viewBox="0 0 24 24"><path d="M3 3h18v18H3z"/><path d="M3 9h18M9 21V9"/></svg>
        React.js-mini-projects
      </div>
      <div class="pinned-desc">Frontend React mini projects covering various UI patterns</div>
      <div class="pinned-foot">
        <div class="lang-dot lang-js"></div> JavaScript
        <span>⭐ 1</span>
      </div>
    </a>
    <a class="pinned-card" href="https://github.com/LSGAMING281004/Jarvis" target="_blank">
      <div class="pinned-name">
        <svg width="14" height="14" fill="none" stroke="var(--cyan)" stroke-width="2" viewBox="0 0 24 24"><path d="M3 3h18v18H3z"/><path d="M3 9h18M9 21V9"/></svg>
        Jarvis
      </div>
      <div class="pinned-desc">Voice Assistant — Android AI app with intent processing</div>
      <div class="pinned-foot">
        <div class="lang-dot lang-java"></div> Java
        <span>⭐ 1</span>
      </div>
    </a>
    <a class="pinned-card" href="https://github.com/LSGAMING281004/ChatBot" target="_blank">
      <div class="pinned-name">
        <svg width="14" height="14" fill="none" stroke="var(--cyan)" stroke-width="2" viewBox="0 0 24 24"><path d="M3 3h18v18H3z"/><path d="M3 9h18M9 21V9"/></svg>
        ChatBot
      </div>
      <div class="pinned-desc">Simple AI chat bot message system built in Java</div>
      <div class="pinned-foot">
        <div class="lang-dot lang-java"></div> Java
      </div>
    </a>
  </div>

  <!-- ACHIEVEMENTS -->
  <div class="section-header">
    <div class="section-title"><span>04.</span> achievements</div>
    <div class="section-line"></div>
  </div>
  <div class="ach-row" style="margin-bottom:2rem;">
    <div class="ach-badge">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="var(--amber)" stroke="none"><path d="M12 2l2.4 7.4H22l-6.2 4.5 2.4 7.3L12 17l-6.2 4.2 2.4-7.3L2 9.4h7.6z"/></svg>
      <div>
        <span>Pull Shark</span>
        <span class="ach-sub">Merged pull requests</span>
      </div>
    </div>
    <div class="ach-badge">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="var(--amber)" stroke="none"><path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"/></svg>
      <div>
        <span>Quickdraw</span>
        <span class="ach-sub">First PR merged</span>
      </div>
    </div>
    <div class="ach-badge">
      <svg width="18" height="18" fill="none" stroke="var(--green)" stroke-width="2" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>
      <div>
        <span>HackerRank Java</span>
        <span class="ach-sub">Java (Basic) certified</span>
      </div>
    </div>
    <div class="ach-badge">
      <svg width="18" height="18" fill="none" stroke="var(--cyan)" stroke-width="2" viewBox="0 0 24 24"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
      <div>
        <span>LeetCode</span>
        <span class="ach-sub">Active problem solver</span>
      </div>
    </div>
  </div>

  <!-- EDUCATION -->
  <div class="section-header">
    <div class="section-title"><span>05.</span> education</div>
    <div class="section-line"></div>
  </div>
  <div class="edu-card">
    <div class="edu-dot">🎓</div>
    <div style="flex:1;min-width:0">
      <div class="edu-degree">Bachelor of Computer Applications</div>
      <div class="edu-inst">Indo American College, Cheyyar</div>
      <div class="edu-meta">
        <span>2022 – 2025</span>
        <span>·</span>
        <span>Computer Science</span>
      </div>
    </div>
    <div class="edu-score">72%<span>Score</span></div>
  </div>

  <!-- CERTIFICATIONS -->
  <div class="section-header">
    <div class="section-title"><span>06.</span> certifications</div>
    <div class="section-line"></div>
  </div>
  <div class="cert-list">
    <div class="cert-card">
      <div class="cert-icon ci-java">☕</div>
      <div>
        <div class="cert-name">Java Full Stack</div>
        <div class="cert-by">SLA Institute</div>
      </div>
      <div class="cert-year">2025</div>
    </div>
    <div class="cert-card">
      <div class="cert-icon ci-ibm">🔵</div>
      <div>
        <div class="cert-name">IBM JavaScript</div>
        <div class="cert-by">IBM Etrain</div>
      </div>
      <div class="cert-year">2025</div>
    </div>
    <div class="cert-card">
      <div class="cert-icon ci-hr">✅</div>
      <div>
        <div class="cert-name">Java (Basic)</div>
        <div class="cert-by">HackerRank</div>
      </div>
      <div class="cert-year">2025</div>
    </div>
  </div>

  <!-- SOCIAL LINKS -->
  <div class="section-header">
    <div class="section-title"><span>07.</span> connect</div>
    <div class="section-line"></div>
  </div>
  <div class="social-grid">
    <a class="social-link gh-link" href="https://github.com/LSGAMING281004" target="_blank">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0024 12c0-6.63-5.37-12-12-12z"/></svg>
      <div>
        <div>GitHub</div>
        <div class="social-handle">LSGAMING281004</div>
      </div>
    </a>
    <a class="social-link li-link" href="https://www.linkedin.com/in/lingsterlokesh" target="_blank">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
      <div>
        <div>LinkedIn</div>
        <div class="social-handle">lingsterlokesh</div>
      </div>
    </a>
    <a class="social-link lc-link" href="https://leetcode.com/u/Lokesh_k_ls/" target="_blank">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M13.483 0a1.374 1.374 0 0 0-.961.438L7.116 6.226l-3.854 4.126a5.266 5.266 0 0 0-1.209 2.104 5.35 5.35 0 0 0-.125.513 5.527 5.527 0 0 0 .062 2.362 5.83 5.83 0 0 0 .349 1.017 5.938 5.938 0 0 0 1.271 1.818l4.277 4.193.039.038c2.248 2.165 5.852 2.133 8.063-.074l2.396-2.392c.54-.54.54-1.414.003-1.955a1.378 1.378 0 0 0-1.951-.003l-2.396 2.392a3.021 3.021 0 0 1-4.205.038l-.02-.019-4.276-4.193c-.652-.64-.972-1.469-.948-2.263a2.68 2.68 0 0 1 .066-.523 2.545 2.545 0 0 1 .619-1.164L9.13 8.114c1.058-1.134 3.204-1.27 4.43-.278l3.501 2.831c.593.48 1.461.387 1.94-.207a1.384 1.384 0 0 0-.207-1.943l-3.5-2.831c-.8-.647-1.766-1.045-2.774-1.202l2.015-2.158A1.384 1.384 0 0 0 13.483 0zm-2.866 12.815a1.38 1.38 0 0 0-1.38 1.382 1.38 1.38 0 0 0 1.38 1.382H20.79a1.38 1.38 0 0 0 1.38-1.382 1.38 1.38 0 0 0-1.38-1.382z"/></svg>
      <div>
        <div>LeetCode</div>
        <div class="social-handle">Lokesh_k_ls</div>
      </div>
    </a>
    <a class="social-link ig-link" href="https://www.instagram.com/professional_ls" target="_blank">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zM12 0C8.741 0 8.333.014 7.053.072 2.695.272.273 2.69.073 7.052.014 8.333 0 8.741 0 12c0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98C8.333 23.986 8.741 24 12 24c3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98C15.668.014 15.259 0 12 0zm0 5.838a6.162 6.162 0 100 12.324 6.162 6.162 0 000-12.324zM12 16a4 4 0 110-8 4 4 0 010 8zm6.406-11.845a1.44 1.44 0 100 2.881 1.44 1.44 0 000-2.881z"/></svg>
      <div>
        <div>Instagram</div>
        <div class="social-handle">professional_ls</div>
      </div>
    </a>
    <a class="social-link em-link" href="mailto:lsgaming342@gmail.com">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M2 9l10 6 10-6"/></svg>
      <div>
        <div>Email</div>
        <div class="social-handle">lsgaming342@gmail.com</div>
      </div>
    </a>
    <a class="social-link pf-link" href="https://lsgaming281004.github.io/portfolio--Lokesh.k/" target="_blank">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M3 9l9-7 9 7v11a2 2 0 01-2 2H5a2 2 0 01-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg>
      <div>
        <div>Portfolio</div>
        <div class="social-handle">lsgaming281004.github.io</div>
      </div>
    </a>
  </div>

  <!-- FOOTER -->
  <div class="footer">
    <strong>LOKESH K</strong> &nbsp;·&nbsp; Full Stack Java Developer &nbsp;·&nbsp; Cheyyar, Tamil Nadu
    <br><br>
    <span style="font-size:10px;opacity:0.5">Built with ♥ · 2025</span>
  </div>

</div>
</body>
</html>

