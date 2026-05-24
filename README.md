
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Ultimate AI Trip Planning Guide — 30+ Expert Prompts</title>
<meta name="description" content="Stop getting generic AI itineraries. 30+ proven prompts that plan trips with zero backtracking, realistic timing, and verified information. Works with ChatGPT, Claude & more.">
<meta property="og:title" content="The Ultimate AI Trip Planning Guide: 30+ Expert Prompts (2025)">
<meta property="og:description" content="A complete copy-paste prompt system for planning any trip with AI — from destination discovery to departure day. Zero backtracking. Verified itineraries.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;0,900;1,400;1,700&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;1,9..40,300&display=swap" rel="stylesheet">
<style>
:root {
  --ink: #0f0e0c;
  --ink-soft: #3a3832;
  --ink-faint: #8a8680;
  --cream: #f7f4ee;
  --cream-dark: #ede9e0;
  --cream-deeper: #e0dbd0;
  --gold: #b8924a;
  --gold-light: #f5ead8;
  --gold-lighter: #fdf8f0;
  --accent: #c94f2a;
  --accent-soft: #f7e8e3;
  --teal: #1a6b5a;
  --teal-soft: #e3f0ec;
  --white: #ffffff;
  --border: rgba(15,14,12,0.1);
  --border-gold: rgba(184,146,74,0.3);
}

*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

html { scroll-behavior: smooth; }

body {
  font-family: 'DM Sans', sans-serif;
  font-size: 16px;
  line-height: 1.7;
  color: var(--ink);
  background: var(--cream);
  -webkit-font-smoothing: antialiased;
}

/* ── UTILITY ── */
.container { max-width: 1000px; margin: 0 auto; padding: 0 32px; }
.container--narrow { max-width: 720px; margin: 0 auto; padding: 0 32px; }

/* ── NAV ── */
nav {
  background: var(--ink);
  padding: 0 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 56px;
  position: sticky;
  top: 0;
  z-index: 100;
}
.nav-brand {
  font-family: 'Playfair Display', serif;
  font-size: 15px;
  font-weight: 700;
  color: var(--cream);
  letter-spacing: 0.02em;
  text-decoration: none;
}
.nav-cta {
  background: var(--gold);
  color: var(--ink);
  font-size: 13px;
  font-weight: 500;
  padding: 8px 20px;
  border-radius: 2px;
  text-decoration: none;
  letter-spacing: 0.02em;
  transition: background 0.2s;
}
.nav-cta:hover { background: #cfa355; }

/* ── HERO ── */
.hero {
  background: var(--ink);
  position: relative;
  overflow: hidden;
  padding: 80px 32px 72px;
}
.hero::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0; bottom: 0;
  background-image: radial-gradient(circle at 80% 20%, rgba(184,146,74,0.08) 0%, transparent 60%),
                    radial-gradient(circle at 10% 80%, rgba(26,107,90,0.06) 0%, transparent 50%);
}
.hero-inner { max-width: 1000px; margin: 0 auto; position: relative; }

.hero-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 28px;
}
.hero-eyebrow::before {
  content: '';
  display: block;
  width: 32px;
  height: 1px;
  background: var(--gold);
}

.hero-title {
  font-family: 'Playfair Display', serif;
  font-size: clamp(38px, 6vw, 68px);
  font-weight: 900;
  line-height: 1.08;
  color: var(--cream);
  margin-bottom: 12px;
  max-width: 780px;
}
.hero-title em {
  font-style: italic;
  color: var(--gold);
}

.hero-sub {
  font-size: 18px;
  font-weight: 300;
  color: rgba(247,244,238,0.65);
  max-width: 580px;
  line-height: 1.65;
  margin-bottom: 48px;
}

.hero-stats {
  display: flex;
  flex-wrap: wrap;
  gap: 0;
  border: 1px solid rgba(184,146,74,0.25);
  border-radius: 4px;
  overflow: hidden;
  max-width: 640px;
  margin-bottom: 40px;
}
.hero-stat {
  flex: 1;
  min-width: 140px;
  padding: 20px 24px;
  border-right: 1px solid rgba(184,146,74,0.2);
}
.hero-stat:last-child { border-right: none; }
.hero-stat-num {
  font-family: 'Playfair Display', serif;
  font-size: 28px;
  font-weight: 700;
  color: var(--gold);
  line-height: 1;
  margin-bottom: 4px;
}
.hero-stat-label {
  font-size: 12px;
  font-weight: 400;
  color: rgba(247,244,238,0.5);
  letter-spacing: 0.02em;
}

.hero-cta-group { display: flex; align-items: center; gap: 20px; flex-wrap: wrap; }
.btn-primary {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  background: var(--gold);
  color: var(--ink);
  font-size: 15px;
  font-weight: 500;
  padding: 16px 32px;
  border-radius: 2px;
  text-decoration: none;
  letter-spacing: 0.02em;
  transition: all 0.2s;
}
.btn-primary:hover { background: #cfa355; transform: translateY(-1px); }
.btn-primary svg { width: 16px; height: 16px; }
.btn-ghost {
  font-size: 14px;
  font-weight: 400;
  color: rgba(247,244,238,0.55);
  text-decoration: none;
  letter-spacing: 0.02em;
  display: flex;
  align-items: center;
  gap: 6px;
  transition: color 0.2s;
}
.btn-ghost:hover { color: var(--cream); }

/* ── TRUST BAR ── */
.trust-bar {
  background: var(--cream-dark);
  border-bottom: 1px solid var(--border);
  padding: 14px 32px;
}
.trust-bar-inner {
  max-width: 1000px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  gap: 8px 24px;
}
.trust-item {
  display: flex;
  align-items: center;
  gap: 7px;
  font-size: 13px;
  font-weight: 400;
  color: var(--ink-soft);
}
.trust-item svg { width: 14px; height: 14px; color: var(--teal); flex-shrink: 0; }
.trust-sep { color: var(--ink-faint); font-size: 12px; }

/* ── SECTION STRUCTURE ── */
section { padding: 80px 0; }
section + section { border-top: 1px solid var(--border); }

.section-label {
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 14px;
  display: flex;
  align-items: center;
  gap: 10px;
}
.section-label::before { content: ''; display: block; width: 24px; height: 1px; background: var(--gold); }

.section-title {
  font-family: 'Playfair Display', serif;
  font-size: clamp(26px, 4vw, 38px);
  font-weight: 700;
  line-height: 1.2;
  color: var(--ink);
  margin-bottom: 16px;
}
.section-title em { font-style: italic; color: var(--gold); }

.section-body {
  font-size: 16px;
  font-weight: 300;
  color: var(--ink-soft);
  line-height: 1.75;
  max-width: 640px;
}
.section-body p + p { margin-top: 16px; }
.section-body strong { font-weight: 500; color: var(--ink); }

/* ── PROBLEM SECTION ── */
.problem-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1px;
  background: var(--border);
  border: 1px solid var(--border);
  border-radius: 4px;
  overflow: hidden;
  margin-top: 40px;
}
.problem-cell {
  background: var(--white);
  padding: 28px 32px;
}
.problem-icon {
  width: 36px;
  height: 36px;
  background: var(--accent-soft);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 14px;
}
.problem-icon svg { width: 16px; height: 16px; color: var(--accent); }
.problem-title { font-size: 15px; font-weight: 500; color: var(--ink); margin-bottom: 6px; }
.problem-desc { font-size: 14px; font-weight: 300; color: var(--ink-soft); line-height: 1.6; }

/* ── SOLUTION CALLOUT ── */
.solution-callout {
  background: var(--ink);
  border-radius: 4px;
  padding: 40px 48px;
  margin-top: 48px;
  position: relative;
  overflow: hidden;
}
.solution-callout::after {
  content: '"';
  font-family: 'Playfair Display', serif;
  font-size: 240px;
  font-weight: 900;
  color: rgba(184,146,74,0.06);
  position: absolute;
  top: -40px;
  right: 24px;
  line-height: 1;
}
.solution-text {
  font-family: 'Playfair Display', serif;
  font-size: clamp(20px, 3vw, 26px);
  font-weight: 400;
  font-style: italic;
  color: var(--cream);
  line-height: 1.5;
  max-width: 640px;
  position: relative;
  z-index: 1;
}
.solution-text strong { font-style: normal; font-weight: 700; color: var(--gold); }

/* ── WHAT'S INSIDE ── */
.parts-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 1px; background: var(--border); border: 1px solid var(--border); border-radius: 4px; overflow: hidden; margin-top: 48px; }
.part-card { background: var(--white); padding: 32px; position: relative; transition: background 0.2s; }
.part-card:hover { background: var(--gold-lighter); }
.part-num {
  font-family: 'Playfair Display', serif;
  font-size: 11px;
  font-weight: 700;
  letter-spacing: 0.1em;
  color: var(--gold);
  text-transform: uppercase;
  margin-bottom: 10px;
}
.part-title { font-size: 16px; font-weight: 500; color: var(--ink); margin-bottom: 10px; line-height: 1.35; }
.part-desc { font-size: 13.5px; font-weight: 300; color: var(--ink-soft); line-height: 1.65; margin-bottom: 16px; }
.part-prompts {
  display: flex;
  flex-wrap: wrap;
  gap: 5px;
}
.part-prompt-tag {
  font-size: 11px;
  font-weight: 400;
  color: var(--ink-faint);
  background: var(--cream-dark);
  padding: 3px 9px;
  border-radius: 2px;
}

/* ── PROMPT COUNT STRIP ── */
.count-strip {
  background: var(--gold-light);
  border: 1px solid var(--border-gold);
  border-radius: 4px;
  padding: 24px 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 16px;
  margin-top: 48px;
}
.count-strip-title {
  font-family: 'Playfair Display', serif;
  font-size: 20px;
  font-weight: 700;
  color: var(--ink);
}
.count-strip-sub { font-size: 14px; font-weight: 300; color: var(--ink-soft); margin-top: 3px; }
.count-badges { display: flex; flex-wrap: wrap; gap: 8px; }
.count-badge {
  background: var(--white);
  border: 1px solid var(--border-gold);
  border-radius: 2px;
  padding: 6px 14px;
  font-size: 12px;
  font-weight: 500;
  color: var(--ink-soft);
  display: flex;
  align-items: center;
  gap: 6px;
}
.count-badge span { font-family: 'Playfair Display', serif; font-size: 16px; font-weight: 700; color: var(--gold); }

/* ── ACCURACY SECTION ── */
.accuracy-split {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 1px;
  background: var(--border);
  border: 1px solid var(--border);
  border-radius: 4px;
  overflow: hidden;
  margin-top: 48px;
}
.acc-col { background: var(--white); padding: 28px 24px; }
.acc-col-head {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 18px;
  padding-bottom: 14px;
  border-bottom: 1px solid var(--border);
}
.acc-dot { width: 10px; height: 10px; border-radius: 50%; flex-shrink: 0; }
.acc-dot-green { background: #3B6D11; }
.acc-dot-amber { background: var(--gold); }
.acc-dot-red { background: var(--accent); }
.acc-col-label { font-size: 12px; font-weight: 500; color: var(--ink); letter-spacing: 0.03em; }
.acc-item { font-size: 13px; font-weight: 300; color: var(--ink-soft); padding: 5px 0; border-bottom: 1px solid var(--cream-dark); line-height: 1.4; }
.acc-item:last-child { border-bottom: none; }

/* ── FORMAT DEMO ── */
.format-shell {
  background: var(--white);
  border: 1px solid var(--border);
  border-radius: 4px;
  overflow: hidden;
  margin-top: 48px;
  box-shadow: 0 2px 24px rgba(15,14,12,0.06);
}
.format-topbar {
  background: var(--ink);
  padding: 12px 20px;
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 12px;
  color: rgba(247,244,238,0.5);
  font-weight: 300;
}
.format-topbar strong { color: var(--gold); font-weight: 500; }
.format-body { padding: 24px; font-family: 'DM Mono', 'Fira Code', 'Consolas', monospace; }
.fd-day { font-size: 14px; font-weight: 700; color: var(--ink); font-family: 'DM Sans', sans-serif; }
.fd-base { font-size: 12px; color: var(--ink-faint); margin-bottom: 14px; font-family: 'DM Sans', sans-serif; }
.fd-hr { border: none; border-top: 1px solid var(--cream-dark); margin: 12px 0; }
.fd-row { display: flex; gap: 14px; align-items: baseline; margin-bottom: 2px; }
.fd-time { min-width: 46px; font-size: 12px; color: var(--ink-faint); font-weight: 500; }
.fd-place { font-size: 13px; font-weight: 500; color: var(--ink); font-family: 'DM Sans', sans-serif; }
.fd-arrow { display: block; padding-left: 60px; font-size: 12px; color: var(--ink-faint); margin-bottom: 8px; font-family: 'DM Sans', sans-serif; font-weight: 300; }
.fd-badge { display: inline-block; font-size: 10px; font-weight: 500; padding: 2px 7px; border-radius: 2px; font-family: 'DM Sans', sans-serif; margin-left: 5px; vertical-align: middle; letter-spacing: 0.04em; }
.fdb-book { background: var(--gold-light); color: #7a5a1a; border: 1px solid var(--border-gold); }
.fdb-verify { background: #E6F1FB; color: #0C447C; border: 1px solid #85B7EB; }
.fd-totals { font-size: 12px; color: var(--ink-faint); font-family: 'DM Sans', sans-serif; margin-top: 8px; }
.fd-route { font-size: 12px; color: var(--teal); font-family: 'DM Sans', sans-serif; margin-top: 3px; }

/* ── SOURCE TABLE ── */
.source-table-wrap { margin-top: 40px; overflow-x: auto; }
.source-table { width: 100%; border-collapse: collapse; font-size: 13.5px; }
.source-table th { text-align: left; padding: 10px 16px; font-size: 11px; font-weight: 500; letter-spacing: 0.07em; text-transform: uppercase; color: var(--ink-faint); background: var(--cream-dark); border-bottom: 1px solid var(--border); }
.source-table td { padding: 12px 16px; border-bottom: 1px solid var(--border); vertical-align: top; line-height: 1.5; }
.source-table td:first-child { font-weight: 500; color: var(--ink); }
.source-table td:nth-child(2) { color: var(--ink-soft); font-weight: 300; font-size: 13px; }
.source-table tr:hover td { background: var(--cream-dark); }
.live-badge { background: #EAF3DE; color: #27500A; font-size: 11px; font-weight: 500; padding: 2px 8px; border-radius: 2px; white-space: nowrap; }
.semi-badge { background: var(--gold-light); color: #7a5a1a; font-size: 11px; font-weight: 500; padding: 2px 8px; border-radius: 2px; white-space: nowrap; }

/* ── FOR WHO ── */
.audience-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 16px; margin-top: 40px; }
.audience-card {
  background: var(--white);
  border: 1px solid var(--border);
  border-radius: 4px;
  padding: 24px;
  transition: border-color 0.2s, transform 0.2s;
}
.audience-card:hover { border-color: var(--gold); transform: translateY(-2px); }
.audience-icon {
  width: 40px; height: 40px;
  background: var(--gold-light);
  border-radius: 50%;
  display: flex; align-items: center; justify-content: center;
  margin-bottom: 14px;
}
.audience-icon svg { width: 18px; height: 18px; color: var(--gold); }
.audience-title { font-size: 14px; font-weight: 500; color: var(--ink); margin-bottom: 6px; }
.audience-desc { font-size: 13px; font-weight: 300; color: var(--ink-soft); line-height: 1.55; }

/* ── CHECKLIST ── */
.checklist { margin-top: 40px; }
.cl-item { display: flex; gap: 14px; align-items: flex-start; padding: 16px 0; border-bottom: 1px solid var(--border); }
.cl-item:last-child { border-bottom: none; }
.cl-check { width: 22px; height: 22px; background: var(--teal-soft); border-radius: 50%; display: flex; align-items: center; justify-content: center; flex-shrink: 0; margin-top: 2px; }
.cl-check svg { width: 11px; height: 11px; color: var(--teal); }
.cl-title { font-size: 15px; font-weight: 500; color: var(--ink); margin-bottom: 3px; }
.cl-sub { font-size: 13.5px; font-weight: 300; color: var(--ink-soft); line-height: 1.6; }

/* ── TESTIMONIAL ── */
.testimonials { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 1px; background: var(--border); border: 1px solid var(--border); border-radius: 4px; overflow: hidden; margin-top: 48px; }
.testi-card { background: var(--white); padding: 28px; }
.testi-stars { color: var(--gold); font-size: 13px; letter-spacing: 2px; margin-bottom: 12px; }
.testi-quote { font-size: 14px; font-weight: 300; color: var(--ink-soft); line-height: 1.7; margin-bottom: 16px; font-style: italic; }
.testi-name { font-size: 13px; font-weight: 500; color: var(--ink); }
.testi-role { font-size: 12px; font-weight: 300; color: var(--ink-faint); }

/* ── CTA BLOCK ── */
.cta-block {
  background: var(--ink);
  border-radius: 4px;
  padding: 56px 48px;
  text-align: center;
  position: relative;
  overflow: hidden;
}
.cta-block::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0; bottom: 0;
  background-image: radial-gradient(circle at 50% 0%, rgba(184,146,74,0.12) 0%, transparent 60%);
}
.cta-block > * { position: relative; z-index: 1; }
.cta-title {
  font-family: 'Playfair Display', serif;
  font-size: clamp(26px, 4vw, 40px);
  font-weight: 700;
  color: var(--cream);
  margin-bottom: 14px;
  line-height: 1.2;
}
.cta-title em { font-style: italic; color: var(--gold); }
.cta-sub { font-size: 16px; font-weight: 300; color: rgba(247,244,238,0.6); margin-bottom: 36px; max-width: 500px; margin-left: auto; margin-right: auto; line-height: 1.65; }
.cta-includes { display: flex; justify-content: center; flex-wrap: wrap; gap: 20px; margin-bottom: 36px; }
.cta-include { display: flex; align-items: center; gap: 7px; font-size: 13px; color: rgba(247,244,238,0.6); }
.cta-include svg { width: 14px; height: 14px; color: var(--gold); flex-shrink: 0; }

/* ── FAQ ── */
.faq-list { margin-top: 40px; }
.faq-item { border-bottom: 1px solid var(--border); }
.faq-q {
  padding: 20px 0;
  font-size: 15px;
  font-weight: 500;
  color: var(--ink);
  cursor: pointer;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 16px;
  user-select: none;
}
.faq-q:hover { color: var(--gold); }
.faq-icon { width: 18px; height: 18px; flex-shrink: 0; transition: transform 0.25s; color: var(--ink-faint); }
.faq-item.open .faq-icon { transform: rotate(45deg); }
.faq-a { font-size: 14px; font-weight: 300; color: var(--ink-soft); line-height: 1.75; max-height: 0; overflow: hidden; transition: max-height 0.35s ease, padding 0.25s; }
.faq-item.open .faq-a { max-height: 400px; padding-bottom: 20px; }

/* ── FOOTER ── */
footer {
  background: var(--ink);
  padding: 40px 32px;
  text-align: center;
}
.footer-brand {
  font-family: 'Playfair Display', serif;
  font-size: 18px;
  font-weight: 700;
  color: var(--cream);
  margin-bottom: 10px;
}
.footer-note { font-size: 13px; font-weight: 300; color: rgba(247,244,238,0.4); max-width: 480px; margin: 0 auto; line-height: 1.65; }

/* ── ANIMATIONS ── */
@keyframes fadeUp { from { opacity: 0; transform: translateY(24px); } to { opacity: 1; transform: translateY(0); } }
.hero-eyebrow { animation: fadeUp 0.5s ease both; }
.hero-title { animation: fadeUp 0.6s 0.1s ease both; }
.hero-sub { animation: fadeUp 0.6s 0.2s ease both; }
.hero-stats { animation: fadeUp 0.6s 0.3s ease both; }
.hero-cta-group { animation: fadeUp 0.6s 0.4s ease both; }

/* ── RESPONSIVE ── */
@media (max-width: 700px) {
  .hero { padding: 56px 24px 52px; }
  .problem-grid { grid-template-columns: 1fr; }
  .parts-grid { grid-template-columns: 1fr; }
  .accuracy-split { grid-template-columns: 1fr; }
  .testimonials { grid-template-columns: 1fr; }
  .solution-callout { padding: 28px 24px; }
  .cta-block { padding: 40px 24px; }
  .container, .container--narrow { padding: 0 20px; }
  section { padding: 56px 0; }
  nav { padding: 0 20px; }
  .trust-bar { padding: 12px 20px; }
}
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <a href="#" class="nav-brand">AI Trip Planning Guide</a>
  <a href="#get-it" class="nav-cta">Get the guide</a>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-inner">
    <div class="hero-eyebrow">Complete prompt system · 2025 edition</div>
    <h1 class="hero-title">The <em>Ultimate</em> AI Trip<br>Planning Guide</h1>
    <p class="hero-sub">30+ expert prompts that turn ChatGPT, Claude, or any AI tool into a precision trip planner — with zero backtracking, realistic timing, and verified information you can actually trust.</p>

    <div class="hero-stats">
      <div class="hero-stat">
        <div class="hero-stat-num">30+</div>
        <div class="hero-stat-label">Copy-paste prompts</div>
      </div>
      <div class="hero-stat">
        <div class="hero-stat-num">6</div>
        <div class="hero-stat-label">Complete systems</div>
      </div>
      <div class="hero-stat">
        <div class="hero-stat-num">0</div>
        <div class="hero-stat-label">Backtracking routes</div>
      </div>
      <div class="hero-stat">
        <div class="hero-stat-num">Any</div>
        <div class="hero-stat-label">AI tool — it works</div>
      </div>
    </div>

    <div class="hero-cta-group">
      <a href="#get-it" class="btn-primary">
        <svg viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="2"><path d="M8 2v9M4 8l4 4 4-4"/><path d="M2 14h12"/></svg>
        Download the guide
      </a>
      <a href="#whats-inside" class="btn-ghost">
        See what's inside
        <svg width="14" height="14" viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M3 7h8M8 4l3 3-3 3"/></svg>
      </a>
    </div>
  </div>
</section>

<!-- TRUST BAR -->
<div class="trust-bar">
  <div class="trust-bar-inner">
    <div class="trust-item">
      <svg viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 7 6 11 12 3"/></svg>
      Works with ChatGPT, Claude &amp; Gemini
    </div>
    <span class="trust-sep">·</span>
    <div class="trust-item">
      <svg viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 7 6 11 12 3"/></svg>
      No technical knowledge needed
    </div>
    <span class="trust-sep">·</span>
    <div class="trust-item">
      <svg viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 7 6 11 12 3"/></svg>
      Solo trips, families, multi-city — all covered
    </div>
    <span class="trust-sep">·</span>
    <div class="trust-item">
      <svg viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 7 6 11 12 3"/></svg>
      Instant download, use immediately
    </div>
  </div>
</div>

<!-- PROBLEM -->
<section>
  <div class="container">
    <div class="section-label">The problem</div>
    <h2 class="section-title">AI keeps giving you<br><em>bad itineraries.</em></h2>
    <div class="section-body">
      <p>You've asked ChatGPT or Claude to plan a trip. You got back something that looked reasonable — a list of places, some descriptions, a rough schedule. Then you opened a map.</p>
      <p>Day two has you walking from one side of the city to the other, back again, then to a restaurant that closed eight months ago. The museum is scheduled for Monday — the one day it's shut. There's no transit time between stops, which means the whole schedule is fiction.</p>
      <p><strong>The problem isn't the AI. It's the absence of a system.</strong> AI thinks like a travel blogger: thematically grouped, beautifully described, geographically chaotic. To get good itineraries, you need to teach it to think like a route planner.</p>
    </div>

    <div class="problem-grid">
      <div class="problem-cell">
        <div class="problem-icon">
          <svg viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M8 2C5.2 2 3 4.2 3 7c0 3.8 5 9 5 9s5-5.2 5-9c0-2.8-2.2-5-5-5z"/><circle cx="8" cy="7" r="1.5"/></svg>
        </div>
        <div class="problem-title">Backtracking routes</div>
        <div class="problem-desc">AI groups attractions by category, not geography. The result zigzags across the map and wastes hours in transit.</div>
      </div>
      <div class="problem-cell">
        <div class="problem-icon">
          <svg viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="1.5"><circle cx="8" cy="8" r="6"/><path d="M8 5v3l2 2"/></svg>
        </div>
        <div class="problem-title">Impossible timings</div>
        <div class="problem-desc">No transit time between stops. No buffer for queues, meals, or navigation. Days that look fine on paper fall apart by 11am.</div>
      </div>
      <div class="problem-cell">
        <div class="problem-icon">
          <svg viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M2 4h12v10H2z"/><path d="M5 4V2M11 4V2"/><path d="M2 8h12"/></svg>
        </div>
        <div class="problem-title">Closed on arrival</div>
        <div class="problem-desc">AI doesn't check what's closed on which days. Monday museum visits. Saturday-only markets on a Wednesday. All common failures.</div>
      </div>
      <div class="problem-cell">
        <div class="problem-icon">
          <svg viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M8 2l1.5 3 3.5.5-2.5 2.5.6 3.5L8 10l-3.1 1.5.6-3.5L3 5.5 6.5 5z"/></svg>
        </div>
        <div class="problem-title">Outdated information</div>
        <div class="problem-desc">AI has a knowledge cutoff. It confidently lists restaurants that closed, attractions that changed hours, and visa rules that no longer apply.</div>
      </div>
    </div>

    <div class="solution-callout">
      <p class="solution-text">The difference between asking AI for an itinerary and getting a <strong>good</strong> itinerary is a structured system of prompts that teaches it to think spatially, account for real time, and tell you exactly what to verify.</p>
    </div>
  </div>
</section>

<!-- WHAT'S INSIDE -->
<section id="whats-inside">
  <div class="container">
    <div class="section-label">What's inside</div>
    <h2 class="section-title">Six complete systems.<br><em>Every stage covered.</em></h2>
    <div class="section-body">
      <p>This isn't a collection of generic travel questions to paste into ChatGPT. It's a sequential, interlocking prompt system — each step feeds the next, and skipping steps is exactly what causes bad itineraries.</p>
    </div>

    <div class="parts-grid">
      <div class="part-card">
        <div class="part-num">Part 01</div>
        <div class="part-title">Destination discovery</div>
        <div class="part-desc">Prompts to find the right destination for your exact travel style, compare shortlists head-to-head, and surface genuinely off-the-beaten-path options most travellers never consider.</div>
        <div class="part-prompts">
          <span class="part-prompt-tag">Destination matcher</span>
          <span class="part-prompt-tag">Head-to-head compare</span>
          <span class="part-prompt-tag">Hidden gem finder</span>
        </div>
      </div>
      <div class="part-card">
        <div class="part-num">Part 02</div>
        <div class="part-title">Single-city optimised itinerary</div>
        <div class="part-desc">The core 6-step framework. Geographic clustering, honest time budgeting, day-by-day route building, and a full audit — all structured to eliminate backtracking before it ever happens.</div>
        <div class="part-prompts">
          <span class="part-prompt-tag">Data dump</span>
          <span class="part-prompt-tag">Geo clustering</span>
          <span class="part-prompt-tag">Time mapping</span>
          <span class="part-prompt-tag">Day builder</span>
          <span class="part-prompt-tag">Full audit</span>
        </div>
      </div>
      <div class="part-card">
        <div class="part-num">Part 03</div>
        <div class="part-title">Multi-city macro routing</div>
        <div class="part-desc">Solve city order as a routing problem first. Includes city sequence optimisation, days-per-city allocation with real transit costs, per-leg journey planning, and a sanity check that tells you when a trip is simply too ambitious.</div>
        <div class="part-prompts">
          <span class="part-prompt-tag">City order solver</span>
          <span class="part-prompt-tag">Days allocation</span>
          <span class="part-prompt-tag">Transit planning</span>
          <span class="part-prompt-tag">Macro audit</span>
        </div>
      </div>
      <div class="part-card">
        <div class="part-num">Part 04</div>
        <div class="part-title">AI accuracy &amp; verification</div>
        <div class="part-desc">A complete guide to what AI gets right versus what it gets wrong — and a trusted source directory for 14 types of travel information. Prompts that make AI flag its own uncertainty so you know exactly what to check.</div>
        <div class="part-prompts">
          <span class="part-prompt-tag">Confidence flags</span>
          <span class="part-prompt-tag">Source directory</span>
          <span class="part-prompt-tag">Verification checklist</span>
        </div>
      </div>
      <div class="part-card">
        <div class="part-num">Part 05</div>
        <div class="part-title">Itinerary format standard</div>
        <div class="part-desc">The definitive format for AI-generated itineraries — specific times, transit arrows between every stop, verification badges, and a 10-point quality checklist. Never accept a substandard plan again.</div>
        <div class="part-prompts">
          <span class="part-prompt-tag">Format request</span>
          <span class="part-prompt-tag">Quality checklist</span>
          <span class="part-prompt-tag">Self-audit prompt</span>
        </div>
      </div>
      <div class="part-card">
        <div class="part-num">Part 06</div>
        <div class="part-title">Logistics, budget &amp; packing</div>
        <div class="part-desc">Accommodation strategy, local transport planning, realistic budget breakdowns, money-saving tactics, custom packing lists, pre-departure timelines, and on-trip real-time prompts for when plans change.</div>
        <div class="part-prompts">
          <span class="part-prompt-tag">Budget breakdown</span>
          <span class="part-prompt-tag">Packing list</span>
          <span class="part-prompt-tag">Pre-trip checklist</span>
          <span class="part-prompt-tag">On-trip help</span>
        </div>
      </div>
    </div>

    <div class="count-strip">
      <div>
        <div class="count-strip-title">Everything in the guide</div>
        <div class="count-strip-sub">A complete system — not a list of questions</div>
      </div>
      <div class="count-badges">
        <div class="count-badge"><span>30+</span> copy-paste prompts</div>
        <div class="count-badge"><span>6</span> complete systems</div>
        <div class="count-badge"><span>14</span> verified source types</div>
        <div class="count-badge"><span>10-pt</span> quality checklist</div>
      </div>
    </div>
  </div>
</section>

<!-- FORMAT DEMO -->
<section style="background: var(--cream-dark);">
  <div class="container">
    <div class="section-label">What you'll produce</div>
    <h2 class="section-title">Itineraries that look<br><em>like this.</em></h2>
    <div class="section-body">
      <p>Every prompt in the guide is engineered to produce output in this format: specific clock times, transit minutes between every stop, verification badges on anything that needs checking, and a route logic statement confirming there's no backtracking. This is what a trustworthy AI itinerary actually looks like.</p>
    </div>

    <div class="format-shell">
      <div class="format-topbar">
        <strong>Day 2 — Tuesday 15 July · Rome: Ancient Centre</strong> &nbsp;·&nbsp; example output
      </div>
      <div class="format-body">
        <div class="fd-day">Day 2 — Tuesday 15 July · Rome: Ancient Centre</div>
        <div class="fd-base">Base: Hotel Navona, Piazza Navona · Transport today: Walking + 1 metro</div>
        <div class="fd-hr"></div>
        <div class="fd-row"><span class="fd-time">08:00</span><span class="fd-place">Breakfast — Bar San Calisto <span class="fd-badge fdb-verify">VERIFY OPEN</span></span></div>
        <span class="fd-arrow">↳ 2 min walk from hotel · Cash only · ~€3 · cornetto + cappuccino</span>
        <div class="fd-row"><span class="fd-time">09:00</span><span class="fd-place">Roman Forum &amp; Palatine Hill <span class="fd-badge fdb-book">BOOK AHEAD</span> <span class="fd-badge fdb-verify">VERIFY PRICE</span></span></div>
        <span class="fd-arrow">↳ 18 min walk · Est. €16 · Allow 2 hrs · Enter via Via Sacra · Last entry 1 hr before close</span>
        <div class="fd-row"><span class="fd-time">11:15</span><span class="fd-place">Colosseum <span class="fd-badge fdb-book">BOOK AHEAD</span></span></div>
        <span class="fd-arrow">↳ 5 min walk · Included in Forum combo · Allow 1.5 hrs · Very hot after midday — go now</span>
        <div class="fd-row"><span class="fd-time">13:00</span><span class="fd-place">Lunch — Osteria da Fortunata <span class="fd-badge fdb-verify">VERIFY OPEN</span></span></div>
        <span class="fd-arrow">↳ 8 min walk · ~€15pp · No reservations — arrive before 1pm to beat the queue</span>
        <div class="fd-row"><span class="fd-time">14:15</span><span class="fd-place">Capitoline Museums <span class="fd-badge fdb-verify">CHECK HOURS</span></span></div>
        <span class="fd-arrow">↳ 6 min walk · Est. €15 · Allow 1.5–2 hrs · Less crowded than Vatican · Don't miss the Marcus Aurelius statue</span>
        <div class="fd-row"><span class="fd-time">16:15</span><span class="fd-place">Walk north via Via del Corso — gelato stop en route</span></div>
        <span class="fd-arrow">↳ 25 min leisurely walk back toward hotel</span>
        <div class="fd-row"><span class="fd-time">20:00</span><span class="fd-place">Dinner — Da Enzo al 29 <span class="fd-badge fdb-book">BOOK AHEAD</span> <span class="fd-badge fdb-verify">VERIFY OPEN TUE</span></span></div>
        <span class="fd-arrow">↳ 12 min walk or taxi ~€8 · Best cacio e pepe in Trastevere · Reserve 2 weeks ahead</span>
        <div class="fd-hr"></div>
        <div class="fd-totals">Day totals: ~5.5km walked · ~€65pp excl. dinner · 2 advance bookings needed</div>
        <div class="fd-route">✓ Route: hotel → SE to Forum → W to Capitoline → N walk home → S to Trastevere (linear, no backtrack)</div>
      </div>
    </div>
  </div>
</section>

<!-- ACCURACY -->
<section>
  <div class="container">
    <div class="section-label">AI accuracy guide</div>
    <h2 class="section-title">Know what to trust.<br><em>Know what to check.</em></h2>
    <div class="section-body">
      <p>Every AI tool has a knowledge cutoff. Opening hours, visa rules, restaurant closures, transport fares — all of these can be outdated the moment you use them. The guide includes a full framework for knowing exactly when to trust AI output and exactly where to go to verify it.</p>
    </div>

    <div class="accuracy-split">
      <div class="acc-col">
        <div class="acc-col-head">
          <div class="acc-dot acc-dot-green"></div>
          <div class="acc-col-label">Trust AI directly</div>
        </div>
        <div class="acc-item">Geographic relationships</div>
        <div class="acc-item">Routing &amp; clustering logic</div>
        <div class="acc-item">Cultural context &amp; customs</div>
        <div class="acc-item">Seasonal weather patterns</div>
        <div class="acc-item">Neighbourhood character</div>
        <div class="acc-item">Activity time estimates</div>
        <div class="acc-item">Travel style matching</div>
      </div>
      <div class="acc-col">
        <div class="acc-col-head">
          <div class="acc-dot acc-dot-amber"></div>
          <div class="acc-col-label">Verify before relying</div>
        </div>
        <div class="acc-item">Opening hours</div>
        <div class="acc-item">Entry prices</div>
        <div class="acc-item">Restaurant operating status</div>
        <div class="acc-item">Transport schedules</div>
        <div class="acc-item">Booking requirements</div>
        <div class="acc-item">Queue &amp; crowd times</div>
        <div class="acc-item">New transport lines</div>
      </div>
      <div class="acc-col">
        <div class="acc-col-head">
          <div class="acc-dot acc-dot-red"></div>
          <div class="acc-col-label">Always verify officially</div>
        </div>
        <div class="acc-item">Visa &amp; entry requirements</div>
        <div class="acc-item">Health &amp; vaccination rules</div>
        <div class="acc-item">Travel safety advisories</div>
        <div class="acc-item">Currency exchange rates</div>
        <div class="acc-item">Border crossing rules</div>
        <div class="acc-item">Political/safety situation</div>
        <div class="acc-item">Drone &amp; photography laws</div>
      </div>
    </div>

    <div class="source-table-wrap">
      <table class="source-table">
        <thead>
          <tr><th>Data type</th><th>Official source to use</th><th>Reliability</th></tr>
        </thead>
        <tbody>
          <tr><td>Visa requirements</td><td>Your government's official travel portal (travel.state.gov · gov.uk/foreign-travel-advice · smartraveller.gov.au)</td><td><span class="live-badge">Live</span></td></tr>
          <tr><td>Opening hours &amp; prices</td><td>Official attraction website or Google Maps verified listing</td><td><span class="live-badge">Live</span></td></tr>
          <tr><td>Train schedules</td><td>National rail operator (Trainline for Europe · Amtrak for US · JR Pass for Japan)</td><td><span class="live-badge">Live</span></td></tr>
          <tr><td>Local transport</td><td>City transport authority official app (TfL · RATP · MTA etc.)</td><td><span class="live-badge">Live</span></td></tr>
          <tr><td>Restaurant status</td><td>Google Maps (check "permanently closed") + TripAdvisor last 3 months</td><td><span class="semi-badge">Semi-live</span></td></tr>
          <tr><td>Health &amp; vaccinations</td><td>CDC (cdc.gov/travel), WHO, or your national health authority</td><td><span class="live-badge">Live</span></td></tr>
          <tr><td>Crowd &amp; wait times</td><td>Google Maps "popular times" graph on each attraction's listing</td><td><span class="semi-badge">Semi-live</span></td></tr>
        </tbody>
      </table>
    </div>
  </div>
</section>

<!-- WHO IT'S FOR -->
<section style="background: var(--cream-dark);">
  <div class="container">
    <div class="section-label">Who it's for</div>
    <h2 class="section-title">Built for every kind<br>of <em>traveller.</em></h2>
    <div class="section-body">
      <p>Whether you're planning a solo weekend break or a three-week multi-country trip for a family of four, the system adapts. Fill in the brackets and go.</p>
    </div>

    <div class="audience-grid">
      <div class="audience-card">
        <div class="audience-icon">
          <svg viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="1.5"><circle cx="9" cy="5" r="3"/><path d="M3 17c0-3.3 2.7-6 6-6s6 2.7 6 6"/></svg>
        </div>
        <div class="audience-title">Solo travellers</div>
        <div class="audience-desc">Build efficient, flexible itineraries for one — optimised for your pace, your interests, and your budget.</div>
      </div>
      <div class="audience-card">
        <div class="audience-icon">
          <svg viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="1.5"><circle cx="6" cy="5" r="2.5"/><circle cx="12" cy="5" r="2.5"/><path d="M1 17c0-2.8 2.2-5 5-5M17 17c0-2.8-2.2-5-5-5M6 12h6"/></svg>
        </div>
        <div class="audience-title">Couples &amp; friends</div>
        <div class="audience-desc">Balance different preferences within a single plan. The constraint prompts handle competing must-dos without the argument.</div>
      </div>
      <div class="audience-card">
        <div class="audience-icon">
          <svg viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="1.5"><rect x="3" y="3" width="12" height="12" rx="2"/><path d="M3 8h12M8 8v7"/></svg>
        </div>
        <div class="audience-title">Families with kids</div>
        <div class="audience-desc">The energy curve and pace constraints are built for this. Flag your children's ages and the system adapts activity selection and timing.</div>
      </div>
      <div class="audience-card">
        <div class="audience-icon">
          <svg viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M9 2L3 6v10h4v-5h4v5h4V6z"/></svg>
        </div>
        <div class="audience-title">Multi-city explorers</div>
        <div class="audience-desc">The macro routing system solves city sequence as a logistics problem first — so your grand tour doesn't zigzag across a continent.</div>
      </div>
      <div class="audience-card">
        <div class="audience-icon">
          <svg viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M2 14l4-4 3 3 4-5 3 3"/><rect x="2" y="2" width="14" height="14" rx="1"/></svg>
        </div>
        <div class="audience-title">Travel creators</div>
        <div class="audience-desc">Build and verify itinerary content for your audience at scale. The format standard ensures consistent, trustworthy output every time.</div>
      </div>
      <div class="audience-card">
        <div class="audience-icon">
          <svg viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="1.5"><rect x="2" y="3" width="14" height="12" rx="1"/><path d="M6 3V2M12 3V2M2 8h14"/></svg>
        </div>
        <div class="audience-title">Business travellers</div>
        <div class="audience-desc">Maximise limited free time around meetings. The partial-day and time-block prompts are built for exactly this situation.</div>
      </div>
    </div>
  </div>
</section>

<!-- WHY DIFFERENT -->
<section>
  <div class="container--narrow">
    <div class="section-label">Why this is different</div>
    <h2 class="section-title">A system, not a<br><em>list of questions.</em></h2>
    <div class="section-body">
      <p>Most AI travel prompt guides give you 10 questions to copy and paste. This guide gives you a framework — a structured sequence where each prompt builds on the previous one, catches its own mistakes, and produces output you can rely on.</p>
    </div>

    <div class="checklist">
      <div class="cl-item">
        <div class="cl-check"><svg viewBox="0 0 11 11" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 6 4.5 8.5 9 3"/></svg></div>
        <div>
          <div class="cl-title">Geographic routing first, always</div>
          <div class="cl-sub">The system forces AI to cluster attractions by location before building any day plan. This is the only way to structurally eliminate backtracking — not fix it afterward.</div>
        </div>
      </div>
      <div class="cl-item">
        <div class="cl-check"><svg viewBox="0 0 11 11" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 6 4.5 8.5 9 3"/></svg></div>
        <div>
          <div class="cl-title">Honest time budgeting built in</div>
          <div class="cl-sub">AI underestimates dwell time and ignores transit gaps. The time mapping step forces explicit time estimates for every stop and every transition — before any day is scheduled.</div>
        </div>
      </div>
      <div class="cl-item">
        <div class="cl-check"><svg viewBox="0 0 11 11" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 6 4.5 8.5 9 3"/></svg></div>
        <div>
          <div class="cl-title">Built to self-audit</div>
          <div class="cl-sub">Every stage has an audit prompt that catches the failures of the previous stage. By the time you have a final itinerary, it's been stress-tested for routing, timing, energy, and practical issues.</div>
        </div>
      </div>
      <div class="cl-item">
        <div class="cl-check"><svg viewBox="0 0 11 11" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 6 4.5 8.5 9 3"/></svg></div>
        <div>
          <div class="cl-title">Verification is part of the system</div>
          <div class="cl-sub">Most prompt guides ignore the accuracy problem entirely. This one has a dedicated layer: prompts that make AI tag its own uncertain facts, plus a source directory telling you exactly where to check each type of information.</div>
        </div>
      </div>
      <div class="cl-item">
        <div class="cl-check"><svg viewBox="0 0 11 11" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 6 4.5 8.5 9 3"/></svg></div>
        <div>
          <div class="cl-title">Works for single cities and multi-country trips</div>
          <div class="cl-sub">The multi-city macro layer solves city sequence, transit legs, and day allocation before any per-city planning begins — the extra problem that most multi-city trips get completely wrong.</div>
        </div>
      </div>
      <div class="cl-item">
        <div class="cl-check"><svg viewBox="0 0 11 11" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 6 4.5 8.5 9 3"/></svg></div>
        <div>
          <div class="cl-title">Tool-agnostic — works with any AI</div>
          <div class="cl-sub">Every prompt in the guide works identically with ChatGPT (any version), Claude, Gemini, Perplexity, and any other conversational AI. The system is built around prompt structure, not platform quirks.</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- TESTIMONIALS -->
<section style="background: var(--cream-dark);">
  <div class="container">
    <div class="section-label">What people say</div>
    <h2 class="section-title">Real trips. Real results.</h2>

    <div class="testimonials">
      <div class="testi-card">
        <div class="testi-stars">★★★★★</div>
        <div class="testi-quote">"I'd tried using ChatGPT for travel planning before and always ended up doing it all manually anyway. This guide completely changed that. The geo clustering step alone saved us two hours of wasted walking on our first day in Lisbon."</div>
        <div class="testi-name">Sarah K.</div>
        <div class="testi-role">Solo traveller · 12 countries in 2024</div>
      </div>
      <div class="testi-card">
        <div class="testi-stars">★★★★★</div>
        <div class="testi-quote">"We used this for a 3-week Japan trip covering Tokyo, Kyoto, Osaka, Hiroshima and Hakone. The multi-city routing section alone is worth 10x the price. We had a logical arc, zero transit waste, and the right number of days in each city."</div>
        <div class="testi-name">Marcus &amp; Priya T.</div>
        <div class="testi-role">Couple · First trip to Japan</div>
      </div>
      <div class="testi-card">
        <div class="testi-stars">★★★★★</div>
        <div class="testi-quote">"As a travel blogger I've been using AI tools for research for a while. The verification framework in this guide is something I genuinely hadn't thought through systematically before. It's changed how I fact-check everything I publish."</div>
        <div class="testi-name">Elena R.</div>
        <div class="testi-role">Travel creator · 85K followers</div>
      </div>
    </div>
  </div>
</section>

<!-- FAQ -->
<section>
  <div class="container--narrow">
    <div class="section-label">Common questions</div>
    <h2 class="section-title">Everything you want<br>to know <em>before</em> you buy.</h2>

    <div class="faq-list">
      <div class="faq-item">
        <div class="faq-q" onclick="toggleFaq(this)">
          Which AI tools does this work with?
          <svg class="faq-icon" viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="2"><line x1="9" y1="3" x2="9" y2="15"/><line x1="3" y1="9" x2="15" y2="9"/></svg>
        </div>
        <div class="faq-a">Every prompt in the guide works with ChatGPT (GPT-4o and later), Claude (all versions), Google Gemini, Perplexity, and any other conversational AI tool. The prompts are built around clear instruction structure, not platform-specific features. If the AI tool accepts text prompts, this guide works with it.</div>
      </div>
      <div class="faq-item">
        <div class="faq-q" onclick="toggleFaq(this)">
          Do I need any technical knowledge to use this?
          <svg class="faq-icon" viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="2"><line x1="9" y1="3" x2="9" y2="15"/><line x1="3" y1="9" x2="15" y2="9"/></svg>
        </div>
        <div class="faq-a">None at all. Every prompt has clear placeholders in brackets — you fill them in with your trip details and paste. The guide also explains the reasoning behind each step so you understand what it's doing and can adapt it if needed. If you can type and copy-paste, you can use this guide.</div>
      </div>
      <div class="faq-item">
        <div class="faq-q" onclick="toggleFaq(this)">
          Can AI travel information be trusted?
          <svg class="faq-icon" viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="2"><line x1="9" y1="3" x2="9" y2="15"/><line x1="3" y1="9" x2="15" y2="9"/></svg>
        </div>
        <div class="faq-a">AI is excellent for structural planning: geographic logic, routing, time estimation, cultural context. It is unreliable for live operational data: opening hours, prices, whether a restaurant still exists, current visa rules. This guide has an entire dedicated section on exactly this distinction, including a trusted source directory and prompts that make AI flag which facts need independent verification before you rely on them.</div>
      </div>
      <div class="faq-item">
        <div class="faq-q" onclick="toggleFaq(this)">
          Does this work for multi-city and multi-country trips?
          <svg class="faq-icon" viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="2"><line x1="9" y1="3" x2="9" y2="15"/><line x1="3" y1="9" x2="15" y2="9"/></svg>
        </div>
        <div class="faq-a">Yes — Part 3 of the guide is dedicated entirely to multi-city planning. It covers city sequence optimisation (treating it as a routing problem, not a preference question), how to allocate days per city accounting for the real cost of transit days, per-leg journey planning, and a full end-to-end trip audit that checks routing efficiency, pace realism, experience diversity, and transit risk across the whole trip.</div>
      </div>
      <div class="faq-item">
        <div class="faq-q" onclick="toggleFaq(this)">
          What format does the guide come in?
          <svg class="faq-icon" viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="2"><line x1="9" y1="3" x2="9" y2="15"/><line x1="3" y1="9" x2="15" y2="9"/></svg>
        </div>
        <div class="faq-a">The guide is delivered as a single HTML file that works in any browser — on desktop, tablet, or phone. Every prompt has a one-click copy button so you can paste directly into your AI tool of choice. The file also prints cleanly as a PDF if you prefer a physical copy. No app, no subscription, no account required.</div>
      </div>
      <div class="faq-item">
        <div class="faq-q" onclick="toggleFaq(this)">
          Will this still work as AI tools get updated?
          <svg class="faq-icon" viewBox="0 0 18 18" fill="none" stroke="currentColor" stroke-width="2"><line x1="9" y1="3" x2="9" y2="15"/><line x1="3" y1="9" x2="15" y2="9"/></svg>
        </div>
        <div class="faq-a">Yes. The system is built on prompt engineering principles that work because of how large language models process instructions — not because of quirks in a specific model version. As AI tools improve, the outputs will get better, not worse. The verification framework is also deliberately tool-agnostic: it routes you to official live sources for anything AI can't reliably know, regardless of how capable the AI becomes.</div>
      </div>
    </div>
  </div>
</section>

<!-- CTA -->
<section id="get-it" style="background: var(--cream-dark); border-top: 1px solid var(--border);">
  <div class="container--narrow">
    <div class="cta-block">
      <h2 class="cta-title">Stop wasting trips on<br><em>AI that guesses.</em></h2>
      <p class="cta-sub">Get the complete system that turns any AI tool into a precision trip planner — geographically optimised, realistically timed, and built on verified information.</p>
      <div class="cta-includes">
        <div class="cta-include">
          <svg viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 7 6 11 12 3"/></svg>
          30+ copy-paste prompts
        </div>
        <div class="cta-include">
          <svg viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 7 6 11 12 3"/></svg>
          6 complete systems
        </div>
        <div class="cta-include">
          <svg viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 7 6 11 12 3"/></svg>
          Verification framework
        </div>
        <div class="cta-include">
          <svg viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 7 6 11 12 3"/></svg>
          Instant download
        </div>
        <div class="cta-include">
          <svg viewBox="0 0 14 14" fill="none" stroke="currentColor" stroke-width="2"><polyline points="2 7 6 11 12 3"/></svg>
          Works with any AI tool
        </div>
      </div>
      <a href="#" class="btn-primary" style="font-size:16px; padding:18px 40px; margin: 0 auto;">
        <svg viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="2"><path d="M8 2v9M4 8l4 4 4-4"/><path d="M2 14h12"/></svg>
        Get the guide now
      </a>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-brand">The Ultimate AI Trip Planning Guide</div>
  <p class="footer-note">Use AI for structure and logic. Verify all operational facts — opening hours, visa requirements, prices — via official sources before making any booking or travel decision.</p>
</footer>

<script>
function toggleFaq(el) {
  const item = el.parentElement;
  const isOpen = item.classList.contains('open');
  document.querySelectorAll('.faq-item').forEach(i => i.classList.remove('open'));
  if (!isOpen) item.classList.add('open');
}
</script>

</body>
</html>
