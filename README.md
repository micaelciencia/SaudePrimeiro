<!DOCTYPE html>
<html lang="pt-PT">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Raízes — Nutrição Ancestral, Ciência Moderna · Micael Ciência</title>
<meta name="description" content="Plataforma educativa baseada em evidência científica sobre dietas low-carb, cetogénicas e carnívoras. Planos alimentares, suplementação por patologia e repositório de estudos.">
<style>
  :root {
    --navy: #1a2942;
    --navy-deep: #0f1c30;
    --navy-soft: #243a5c;
    --orange: #f5a623;
    --orange-deep: #e89312;
    --cream: #faf7f2;
    --bg: #f4f5f7;
    --text: #2c3e50;
    --text-soft: #5a6577;
    --border: #e1e5eb;
    --green: #4a7c59;
    --red: #b94a48;
    --shadow: 0 4px 24px rgba(26, 41, 66, 0.08);
    --shadow-lg: 0 12px 48px rgba(26, 41, 66, 0.15);
  }
 
  * { margin: 0; padding: 0; box-sizing: border-box; }
 
  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Helvetica Neue", Arial, sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.65;
    -webkit-font-smoothing: antialiased;
  }
 
  .container {
    max-width: 1180px;
    margin: 0 auto;
    padding: 0 24px;
  }
 
  /* ============ NAV ============ */
  nav {
    background: var(--navy);
    padding: 18px 0;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 12px rgba(0,0,0,0.15);
  }
  nav .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 16px;
  }
  .logo {
    display: flex;
    align-items: center;
    gap: 12px;
    color: white;
    font-weight: 700;
    font-size: 18px;
    letter-spacing: 0.5px;
  }
  .logo-mark {
    width: 38px; height: 38px;
    background: var(--orange);
    border-radius: 50%;
    display: grid;
    place-items: center;
    color: var(--navy);
    font-weight: 800;
    font-size: 16px;
  }
  .nav-links {
    display: flex;
    gap: 28px;
    list-style: none;
    flex-wrap: wrap;
  }
  .nav-links a {
    color: rgba(255,255,255,0.85);
    text-decoration: none;
    font-size: 14px;
    font-weight: 500;
    transition: color 0.2s;
  }
  .nav-links a:hover { color: var(--orange); }
 
  /* ============ HERO ============ */
  .hero {
    background: linear-gradient(135deg, var(--navy) 0%, var(--navy-deep) 100%);
    color: white;
    padding: 100px 0 120px;
    position: relative;
    overflow: hidden;
  }
  .hero::before {
    content: "";
    position: absolute;
    top: -50%; right: -10%;
    width: 600px; height: 600px;
    background: radial-gradient(circle, rgba(245,166,35,0.08) 0%, transparent 70%);
    border-radius: 50%;
  }
  .hero-content {
    position: relative;
    z-index: 1;
    max-width: 820px;
  }
  .hero-tag {
    display: inline-block;
    background: rgba(245,166,35,0.15);
    color: var(--orange);
    padding: 8px 18px;
    border-radius: 50px;
    font-size: 13px;
    font-weight: 600;
    letter-spacing: 1.2px;
    text-transform: uppercase;
    margin-bottom: 24px;
  }
  .hero h1 {
    font-size: clamp(2.2rem, 5vw, 3.6rem);
    font-weight: 800;
    line-height: 1.15;
    margin-bottom: 24px;
    letter-spacing: -1px;
  }
  .hero h1 span { color: var(--orange); }
  .hero-lead {
    font-size: 19px;
    color: rgba(255,255,255,0.82);
    margin-bottom: 36px;
    max-width: 680px;
  }
  .hero-cta {
    display: flex;
    gap: 16px;
    flex-wrap: wrap;
  }
  .btn {
    display: inline-block;
    padding: 14px 28px;
    border-radius: 8px;
    font-weight: 600;
    text-decoration: none;
    cursor: pointer;
    border: none;
    font-size: 15px;
    transition: all 0.2s;
    font-family: inherit;
  }
  .btn-primary {
    background: var(--orange);
    color: var(--navy);
  }
  .btn-primary:hover {
    background: var(--orange-deep);
    transform: translateY(-2px);
    box-shadow: 0 8px 24px rgba(245,166,35,0.3);
  }
  .btn-secondary {
    background: transparent;
    color: white;
    border: 2px solid rgba(255,255,255,0.25);
  }
  .btn-secondary:hover {
    border-color: var(--orange);
    color: var(--orange);
  }
 
  /* ============ DISCLAIMER ============ */
  .disclaimer-bar {
    background: #fff8e7;
    border-bottom: 1px solid #f0deaa;
    padding: 14px 0;
    font-size: 13px;
    color: #6b5618;
    text-align: center;
  }
  .disclaimer-bar strong { color: #4a3c10; }
 
  /* ============ SECTION ============ */
  section.block {
    padding: 90px 0;
  }
  section.block.alt {
    background: white;
  }
  .section-header {
    text-align: center;
    max-width: 720px;
    margin: 0 auto 60px;
  }
  .section-eyebrow {
    color: var(--orange-deep);
    font-size: 13px;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    margin-bottom: 14px;
  }
  .section-title {
    font-size: clamp(1.8rem, 3.5vw, 2.6rem);
    color: var(--navy);
    line-height: 1.2;
    margin-bottom: 18px;
    letter-spacing: -0.5px;
    font-weight: 800;
  }
  .section-sub {
    font-size: 17px;
    color: var(--text-soft);
  }
 
  /* ============ PHILOSOPHY GRID ============ */
  .pillars {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 28px;
  }
  .pillar {
    background: white;
    padding: 36px 30px;
    border-radius: 14px;
    border: 1px solid var(--border);
    transition: all 0.25s;
  }
  .pillar:hover {
    transform: translateY(-4px);
    box-shadow: var(--shadow-lg);
    border-color: var(--orange);
  }
  .pillar-icon {
    width: 56px; height: 56px;
    background: linear-gradient(135deg, var(--orange) 0%, var(--orange-deep) 100%);
    border-radius: 14px;
    display: grid;
    place-items: center;
    color: white;
    font-size: 26px;
    margin-bottom: 22px;
  }
  .pillar h3 {
    color: var(--navy);
    font-size: 19px;
    margin-bottom: 12px;
  }
  .pillar p {
    color: var(--text-soft);
    font-size: 15px;
  }
 
  /* ============ QUOTE BOX ============ */
  .quote-block {
    background: linear-gradient(135deg, var(--navy) 0%, var(--navy-soft) 100%);
    color: white;
    padding: 60px 50px;
    border-radius: 18px;
    margin: 50px 0;
    position: relative;
    border-left: 6px solid var(--orange);
  }
  .quote-block::before {
    content: """;
    position: absolute;
    top: 10px; left: 30px;
    font-size: 90px;
    color: var(--orange);
    opacity: 0.4;
    font-family: Georgia, serif;
    line-height: 1;
  }
  .quote-block blockquote {
    font-style: italic;
    font-size: 22px;
    line-height: 1.5;
    margin-bottom: 18px;
    padding-left: 20px;
  }
  .quote-block cite {
    color: var(--orange);
    font-style: normal;
    font-weight: 600;
    padding-left: 20px;
  }
 
  /* ============ DIET QUIZ ============ */
  .quiz-card {
    background: white;
    border-radius: 18px;
    box-shadow: var(--shadow-lg);
    overflow: hidden;
    max-width: 820px;
    margin: 0 auto;
  }
  .quiz-header {
    background: var(--navy);
    color: white;
    padding: 28px 36px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 12px;
  }
  .quiz-header h3 {
    font-size: 18px;
  }
  .quiz-progress {
    background: rgba(255,255,255,0.15);
    width: 200px;
    height: 6px;
    border-radius: 3px;
    overflow: hidden;
  }
  .quiz-progress-bar {
    background: var(--orange);
    height: 100%;
    width: 20%;
    transition: width 0.3s ease;
  }
  .quiz-body {
    padding: 40px 36px;
    min-height: 380px;
  }
  .quiz-q {
    display: none;
  }
  .quiz-q.active { display: block; animation: fadeIn 0.3s ease; }
  @keyframes fadeIn { from { opacity: 0; transform: translateY(8px); } to { opacity: 1; transform: translateY(0); } }
 
  .quiz-q label.q-label {
    display: block;
    font-size: 14px;
    color: var(--orange-deep);
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 8px;
  }
  .quiz-q h4 {
    color: var(--navy);
    font-size: 24px;
    margin-bottom: 28px;
    line-height: 1.3;
  }
  .options {
    display: grid;
    gap: 12px;
  }
  .option {
    background: var(--bg);
    border: 2px solid transparent;
    padding: 18px 22px;
    border-radius: 12px;
    cursor: pointer;
    transition: all 0.2s;
    font-size: 15px;
    color: var(--text);
    text-align: left;
    width: 100%;
    font-family: inherit;
    display: flex;
    align-items: center;
    gap: 14px;
  }
  .option:hover {
    border-color: var(--orange);
    background: white;
    transform: translateX(4px);
  }
  .option.selected {
    border-color: var(--orange);
    background: #fff8e7;
  }
  .option-check {
    width: 22px; height: 22px;
    border: 2px solid #cfd6df;
    border-radius: 50%;
    flex-shrink: 0;
    display: grid;
    place-items: center;
    transition: all 0.2s;
  }
  .option.selected .option-check {
    border-color: var(--orange);
    background: var(--orange);
    color: white;
  }
  .option.selected .option-check::after {
    content: "✓";
    font-size: 13px;
    font-weight: 700;
  }
 
  .checkbox-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
    gap: 10px;
  }
  .checkbox-grid .option { padding: 14px 16px; font-size: 14px; }
 
  .quiz-footer {
    padding: 24px 36px;
    background: var(--bg);
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-top: 1px solid var(--border);
  }
  .btn-quiz {
    padding: 12px 26px;
    border-radius: 8px;
    border: none;
    font-weight: 600;
    cursor: pointer;
    font-family: inherit;
    font-size: 14px;
    transition: all 0.2s;
  }
  .btn-quiz-prev {
    background: transparent;
    color: var(--text-soft);
  }
  .btn-quiz-prev:hover { color: var(--navy); }
  .btn-quiz-next {
    background: var(--navy);
    color: white;
  }
  .btn-quiz-next:hover { background: var(--orange); color: var(--navy); }
  .btn-quiz-next:disabled {
    opacity: 0.4;
    cursor: not-allowed;
  }
 
  /* ============ RESULT ============ */
  .result-card {
    display: none;
    animation: fadeIn 0.4s ease;
  }
  .result-card.active { display: block; }
  .result-banner {
    background: linear-gradient(135deg, var(--navy) 0%, var(--navy-soft) 100%);
    color: white;
    padding: 40px 36px;
    text-align: center;
  }
  .result-banner .badge {
    display: inline-block;
    background: var(--orange);
    color: var(--navy);
    padding: 6px 18px;
    border-radius: 50px;
    font-weight: 700;
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    margin-bottom: 16px;
  }
  .result-banner h3 {
    font-size: 32px;
    margin-bottom: 12px;
  }
  .result-banner p {
    color: rgba(255,255,255,0.8);
    max-width: 580px;
    margin: 0 auto;
  }
  .result-body {
    padding: 36px;
  }
  .result-section {
    margin-bottom: 32px;
  }
  .result-section h4 {
    color: var(--navy);
    font-size: 17px;
    margin-bottom: 14px;
    padding-bottom: 10px;
    border-bottom: 2px solid var(--orange);
    display: inline-block;
  }
  .principles-list {
    list-style: none;
  }
  .principles-list li {
    padding: 10px 0 10px 28px;
    position: relative;
    color: var(--text);
    font-size: 15px;
  }
  .principles-list li::before {
    content: "✓";
    position: absolute;
    left: 0;
    top: 10px;
    color: var(--orange);
    font-weight: 700;
    font-size: 16px;
  }
 
  .menu-week {
    display: grid;
    gap: 10px;
  }
  .menu-day {
    background: var(--bg);
    padding: 16px 20px;
    border-radius: 10px;
    display: grid;
    grid-template-columns: 110px 1fr;
    gap: 18px;
    align-items: start;
  }
  .menu-day strong {
    color: var(--navy);
    font-weight: 700;
  }
  .menu-meals {
    color: var(--text-soft);
    font-size: 14px;
    line-height: 1.7;
  }
  .menu-meals em { color: var(--orange-deep); font-style: normal; font-weight: 600; }
 
  /* ============ PATHOLOGY MATCHER ============ */
  .matcher-wrap {
    background: white;
    border-radius: 18px;
    box-shadow: var(--shadow-lg);
    padding: 40px;
    max-width: 980px;
    margin: 0 auto;
  }
  .matcher-intro {
    margin-bottom: 28px;
  }
  .matcher-intro h3 {
    color: var(--navy);
    font-size: 22px;
    margin-bottom: 10px;
  }
  .matcher-intro p { color: var(--text-soft); }
  .pathology-search {
    width: 100%;
    padding: 14px 18px;
    border: 2px solid var(--border);
    border-radius: 10px;
    font-size: 15px;
    font-family: inherit;
    margin-bottom: 20px;
    transition: border-color 0.2s;
  }
  .pathology-search:focus {
    outline: none;
    border-color: var(--orange);
  }
  .pathology-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
    gap: 10px;
    margin-bottom: 28px;
  }
  .pathology-chip {
    background: var(--bg);
    border: 2px solid transparent;
    padding: 12px 14px;
    border-radius: 10px;
    cursor: pointer;
    transition: all 0.2s;
    font-size: 14px;
    color: var(--text);
    text-align: left;
    font-family: inherit;
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .pathology-chip:hover {
    border-color: var(--orange);
    background: white;
  }
  .pathology-chip.selected {
    border-color: var(--orange);
    background: #fff8e7;
  }
  .pathology-chip .chip-check {
    width: 18px; height: 18px;
    border: 2px solid #cfd6df;
    border-radius: 4px;
    flex-shrink: 0;
    display: grid;
    place-items: center;
  }
  .pathology-chip.selected .chip-check {
    background: var(--orange);
    border-color: var(--orange);
    color: var(--navy);
  }
  .pathology-chip.selected .chip-check::after {
    content: "✓";
    font-size: 12px;
    font-weight: 700;
  }
 
  .matcher-action {
    text-align: center;
    margin: 24px 0 12px;
  }
  .btn-action {
    background: var(--orange);
    color: var(--navy);
    padding: 14px 36px;
    border-radius: 10px;
    border: none;
    font-weight: 700;
    cursor: pointer;
    font-family: inherit;
    font-size: 15px;
    transition: all 0.2s;
  }
  .btn-action:hover { background: var(--orange-deep); }
  .btn-action:disabled { opacity: 0.4; cursor: not-allowed; }
 
  .recommendations {
    margin-top: 36px;
    display: none;
  }
  .recommendations.active { display: block; }
  .rec-card {
    background: white;
    border: 1px solid var(--border);
    border-left: 5px solid var(--orange);
    border-radius: 12px;
    padding: 26px 28px;
    margin-bottom: 18px;
  }
  .rec-card h4 {
    color: var(--navy);
    font-size: 19px;
    margin-bottom: 6px;
  }
  .rec-card .rec-diet {
    color: var(--orange-deep);
    font-size: 13px;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 14px;
  }
  .rec-card p.rec-rationale {
    color: var(--text-soft);
    font-size: 14px;
    margin-bottom: 16px;
    padding-bottom: 16px;
    border-bottom: 1px dashed var(--border);
  }
  .supplements-table {
    width: 100%;
    font-size: 14px;
    border-collapse: collapse;
  }
  .supplements-table th {
    text-align: left;
    color: var(--navy);
    font-weight: 700;
    padding: 10px 12px 10px 0;
    border-bottom: 2px solid var(--border);
    font-size: 13px;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }
  .supplements-table td {
    padding: 12px 12px 12px 0;
    border-bottom: 1px solid var(--border);
    color: var(--text);
    vertical-align: top;
  }
  .supplements-table td:first-child {
    font-weight: 600;
    color: var(--navy);
    width: 32%;
  }
  .supplements-table td:nth-child(2) {
    color: var(--orange-deep);
    font-weight: 600;
    white-space: nowrap;
    width: 22%;
  }
  .supplements-table td:last-child {
    color: var(--text-soft);
    font-size: 13px;
  }
 
  /* ============ TRANSITION ============ */
  .transition-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 18px;
    margin-top: 40px;
  }
  .week-card {
    background: white;
    border-radius: 14px;
    overflow: hidden;
    border: 1px solid var(--border);
    box-shadow: var(--shadow);
  }
  .week-header {
    background: var(--navy);
    color: white;
    padding: 18px 22px;
    text-align: center;
  }
  .week-header .week-num {
    color: var(--orange);
    font-size: 12px;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 2px;
    margin-bottom: 4px;
  }
  .week-header h4 {
    font-size: 17px;
  }
  .week-body {
    padding: 22px;
  }
  .week-body ul {
    list-style: none;
  }
  .week-body li {
    padding: 7px 0 7px 22px;
    position: relative;
    font-size: 14px;
    color: var(--text);
  }
  .week-body li::before {
    content: "→";
    position: absolute;
    left: 0;
    color: var(--orange);
    font-weight: 700;
  }
 
  .keto-flu-box {
    background: var(--navy);
    color: white;
    border-radius: 16px;
    padding: 40px;
    margin-top: 50px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 40px;
  }
  .keto-flu-box h4 {
    color: var(--orange);
    font-size: 22px;
    margin-bottom: 16px;
  }
  .keto-flu-box p { color: rgba(255,255,255,0.85); font-size: 15px; margin-bottom: 12px; }
  .electrolyte-grid {
    display: grid;
    gap: 14px;
  }
  .electrolyte {
    display: grid;
    grid-template-columns: 90px 1fr;
    align-items: center;
    gap: 16px;
    padding: 14px;
    background: rgba(255,255,255,0.06);
    border-radius: 10px;
  }
  .electrolyte strong {
    color: var(--orange);
    font-size: 15px;
  }
  .electrolyte span {
    color: rgba(255,255,255,0.85);
    font-size: 13px;
  }
 
  /* ============ ESTUDOS / REPOSITÓRIO ============ */
  .studies-filter {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    justify-content: center;
    margin-bottom: 40px;
  }
  .filter-pill {
    background: white;
    border: 2px solid var(--border);
    color: var(--text);
    padding: 9px 18px;
    border-radius: 50px;
    cursor: pointer;
    font-size: 13px;
    font-weight: 600;
    font-family: inherit;
    transition: all 0.2s;
  }
  .filter-pill:hover {
    border-color: var(--orange);
    color: var(--orange-deep);
  }
  .filter-pill.active {
    background: var(--navy);
    color: white;
    border-color: var(--navy);
  }
  .studies-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
    gap: 22px;
  }
  .study-card {
    background: white;
    border-radius: 14px;
    padding: 26px 26px 22px;
    border: 1px solid var(--border);
    border-top: 4px solid var(--orange);
    transition: all 0.25s;
    display: flex;
    flex-direction: column;
  }
  .study-card:hover {
    transform: translateY(-3px);
    box-shadow: var(--shadow-lg);
  }
  .study-tag {
    display: inline-block;
    background: #fff3d6;
    color: var(--orange-deep);
    font-size: 11px;
    font-weight: 700;
    padding: 4px 10px;
    border-radius: 4px;
    text-transform: uppercase;
    letter-spacing: 0.8px;
    margin-bottom: 12px;
    align-self: flex-start;
  }
  .study-card h4 {
    color: var(--navy);
    font-size: 16px;
    line-height: 1.35;
    margin-bottom: 10px;
  }
  .study-meta {
    color: var(--text-soft);
    font-size: 13px;
    margin-bottom: 14px;
    font-style: italic;
  }
  .study-meta strong { color: var(--text); font-style: normal; }
  .study-finding {
    color: var(--text);
    font-size: 14px;
    line-height: 1.6;
    margin-bottom: 18px;
    flex-grow: 1;
  }
  .study-finding strong { color: var(--navy); }
  .study-link {
    color: var(--orange-deep);
    text-decoration: none;
    font-weight: 600;
    font-size: 13px;
    border-top: 1px solid var(--border);
    padding-top: 14px;
    display: inline-flex;
    align-items: center;
    gap: 6px;
    transition: color 0.2s;
  }
  .study-link:hover { color: var(--orange); }
  .study-link::after { content: "→"; transition: transform 0.2s; }
  .study-link:hover::after { transform: translateX(4px); }
 
  .books-row {
    margin-top: 60px;
    background: var(--navy);
    border-radius: 16px;
    padding: 40px;
    color: white;
  }
  .books-row h3 {
    color: var(--orange);
    font-size: 18px;
    margin-bottom: 24px;
    text-transform: uppercase;
    letter-spacing: 1.5px;
  }
  .books-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
    gap: 18px;
  }
  .book {
    background: rgba(255,255,255,0.06);
    padding: 20px;
    border-radius: 10px;
    border-left: 3px solid var(--orange);
  }
  .book h5 {
    color: white;
    font-size: 15px;
    margin-bottom: 6px;
  }
  .book .author {
    color: var(--orange);
    font-size: 12px;
    font-weight: 600;
    margin-bottom: 10px;
  }
  .book p {
    color: rgba(255,255,255,0.75);
    font-size: 13px;
    line-height: 1.5;
  }
 
  /* ============ MANIFESTO / FOOTER PERSONAL ============ */
  .manifesto {
    background: var(--bg);
    padding: 100px 0;
  }
  .manifesto-quote {
    background: white;
    border-left: 6px solid var(--orange);
    padding: 32px 40px;
    border-radius: 0 12px 12px 0;
    box-shadow: var(--shadow);
    margin-bottom: 50px;
    max-width: 880px;
  }
  .manifesto-quote blockquote {
    font-style: italic;
    font-size: 21px;
    color: var(--navy);
    line-height: 1.5;
    margin-bottom: 14px;
  }
  .manifesto-quote cite {
    color: var(--text-soft);
    font-style: normal;
    font-size: 14px;
  }
  .manifesto-grid {
    display: grid;
    grid-template-columns: 320px 1fr;
    gap: 50px;
    align-items: start;
  }
  .manifesto-card {
    background: var(--navy);
    color: white;
    padding: 36px 30px;
    border-radius: 16px;
    text-align: center;
  }
  .manifesto-avatar {
    width: 90px; height: 90px;
    background: var(--orange);
    border-radius: 50%;
    display: grid;
    place-items: center;
    color: var(--navy);
    font-weight: 800;
    font-size: 28px;
    margin: 0 auto 18px;
  }
  .manifesto-card h4 {
    font-size: 22px;
    margin-bottom: 6px;
  }
  .manifesto-card .role {
    color: rgba(255,255,255,0.7);
    font-size: 13px;
    margin-bottom: 22px;
  }
  .manifesto-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    justify-content: center;
    margin-bottom: 26px;
  }
  .manifesto-tags span {
    background: var(--navy-soft);
    padding: 6px 12px;
    border-radius: 6px;
    font-size: 12px;
    color: rgba(255,255,255,0.9);
  }
  .manifesto-stat {
    border-top: 1px solid rgba(255,255,255,0.12);
    padding-top: 18px;
  }
  .manifesto-stat .stat-num {
    color: var(--orange);
    font-size: 22px;
    font-weight: 800;
  }
  .manifesto-stat .stat-label {
    color: rgba(255,255,255,0.6);
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 1.2px;
  }
  .manifesto-text p {
    font-size: 17px;
    color: var(--text);
    margin-bottom: 18px;
    line-height: 1.7;
  }
  .manifesto-text strong { color: var(--navy); font-weight: 700; }
  .manifesto-text em.accent { color: var(--orange-deep); font-style: normal; font-weight: 600; }
 
  /* ============ FOOTER ============ */
  footer {
    background: var(--navy-deep);
    color: rgba(255,255,255,0.6);
    padding: 40px 0;
    text-align: center;
    font-size: 13px;
  }
  footer strong { color: var(--orange); }
  footer .legal {
    margin-top: 14px;
    font-size: 12px;
    color: rgba(255,255,255,0.4);
    max-width: 760px;
    margin-left: auto;
    margin-right: auto;
  }
 
  /* ============ CHAT ASSISTENTE ============ */
  .chat-fab {
    position: fixed;
    bottom: 28px;
    right: 28px;
    width: 64px;
    height: 64px;
    background: var(--orange);
    color: var(--navy);
    border: none;
    border-radius: 50%;
    box-shadow: 0 8px 32px rgba(245, 166, 35, 0.45);
    cursor: pointer;
    z-index: 999;
    display: grid;
    place-items: center;
    font-size: 28px;
    transition: all 0.25s ease;
    animation: chatPulse 2.5s ease-in-out infinite;
  }
  .chat-fab:hover {
    transform: scale(1.08);
    background: var(--orange-deep);
  }
  .chat-fab.hidden { display: none; }
  @keyframes chatPulse {
    0%, 100% { box-shadow: 0 8px 32px rgba(245, 166, 35, 0.45); }
    50% { box-shadow: 0 8px 32px rgba(245, 166, 35, 0.75), 0 0 0 12px rgba(245, 166, 35, 0); }
  }
 
  .chat-fab-label {
    position: absolute;
    right: 80px;
    background: var(--navy);
    color: white;
    padding: 10px 16px;
    border-radius: 10px;
    font-size: 13px;
    font-weight: 600;
    white-space: nowrap;
    box-shadow: var(--shadow-lg);
    opacity: 0;
    transform: translateX(10px);
    pointer-events: none;
    transition: all 0.25s;
  }
  .chat-fab:hover + .chat-fab-label,
  .chat-fab-label:hover {
    opacity: 1;
    transform: translateX(0);
  }
  .chat-fab-label::after {
    content: "";
    position: absolute;
    right: -6px;
    top: 50%;
    transform: translateY(-50%);
    border-left: 6px solid var(--navy);
    border-top: 6px solid transparent;
    border-bottom: 6px solid transparent;
  }
 
  .chat-panel {
    position: fixed;
    bottom: 28px;
    right: 28px;
    width: 400px;
    max-width: calc(100vw - 32px);
    height: 620px;
    max-height: calc(100vh - 56px);
    background: white;
    border-radius: 18px;
    box-shadow: 0 24px 64px rgba(15, 28, 48, 0.35);
    display: none;
    flex-direction: column;
    z-index: 1000;
    overflow: hidden;
    animation: chatOpen 0.3s ease;
  }
  .chat-panel.open { display: flex; }
  @keyframes chatOpen {
    from { opacity: 0; transform: translateY(20px) scale(0.95); }
    to { opacity: 1; transform: translateY(0) scale(1); }
  }
 
  .chat-header {
    background: linear-gradient(135deg, var(--navy) 0%, var(--navy-deep) 100%);
    color: white;
    padding: 18px 20px;
    display: flex;
    align-items: center;
    gap: 14px;
  }
  .chat-avatar {
    width: 42px; height: 42px;
    background: var(--orange);
    border-radius: 50%;
    display: grid;
    place-items: center;
    color: var(--navy);
    font-weight: 800;
    font-size: 17px;
    flex-shrink: 0;
    position: relative;
  }
  .chat-avatar::after {
    content: "";
    position: absolute;
    bottom: 0; right: 0;
    width: 12px; height: 12px;
    background: #4ade80;
    border: 2px solid var(--navy);
    border-radius: 50%;
  }
  .chat-info { flex-grow: 1; min-width: 0; }
  .chat-info h4 {
    font-size: 15px;
    margin-bottom: 2px;
    color: white;
  }
  .chat-info span {
    font-size: 12px;
    color: rgba(255,255,255,0.7);
  }
  .chat-close {
    background: rgba(255,255,255,0.1);
    border: none;
    color: white;
    width: 32px;
    height: 32px;
    border-radius: 8px;
    cursor: pointer;
    font-size: 18px;
    transition: background 0.2s;
  }
  .chat-close:hover { background: rgba(255,255,255,0.2); }
 
  .chat-messages {
    flex-grow: 1;
    overflow-y: auto;
    padding: 22px 20px;
    background: var(--bg);
    display: flex;
    flex-direction: column;
    gap: 14px;
  }
  .chat-messages::-webkit-scrollbar { width: 6px; }
  .chat-messages::-webkit-scrollbar-thumb { background: #cfd6df; border-radius: 3px; }
 
  .msg {
    display: flex;
    gap: 10px;
    max-width: 92%;
    animation: msgIn 0.25s ease;
  }
  @keyframes msgIn { from { opacity: 0; transform: translateY(8px); } to { opacity: 1; transform: translateY(0); } }
 
  .msg-bot { align-self: flex-start; }
  .msg-user { align-self: flex-end; flex-direction: row-reverse; }
 
  .msg-bubble {
    padding: 12px 16px;
    border-radius: 14px;
    font-size: 14px;
    line-height: 1.55;
    box-shadow: 0 2px 8px rgba(15, 28, 48, 0.06);
  }
  .msg-bot .msg-bubble {
    background: white;
    color: var(--text);
    border-bottom-left-radius: 4px;
  }
  .msg-user .msg-bubble {
    background: var(--navy);
    color: white;
    border-bottom-right-radius: 4px;
  }
  .msg-bubble strong { color: var(--navy); }
  .msg-user .msg-bubble strong { color: var(--orange); }
  .msg-bubble ul {
    margin: 8px 0 4px 0;
    padding-left: 18px;
  }
  .msg-bubble li { margin-bottom: 4px; }
  .msg-bubble a {
    color: var(--orange-deep);
    font-weight: 600;
    text-decoration: none;
  }
  .msg-bubble a:hover { text-decoration: underline; }
  .msg-bubble .mini-table {
    background: var(--bg);
    border-radius: 8px;
    padding: 10px 12px;
    margin-top: 10px;
    font-size: 13px;
  }
  .msg-bubble .mini-table-row {
    display: flex;
    justify-content: space-between;
    gap: 12px;
    padding: 4px 0;
  }
  .msg-bubble .mini-table-row strong { color: var(--navy); }
  .msg-bubble .mini-table-row span { color: var(--orange-deep); font-weight: 600; }
 
  .chat-suggestions {
    padding: 0 20px 12px;
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    background: var(--bg);
  }
  .suggestion-chip {
    background: white;
    border: 1px solid var(--border);
    color: var(--navy);
    padding: 8px 12px;
    border-radius: 20px;
    font-size: 12px;
    cursor: pointer;
    font-family: inherit;
    transition: all 0.2s;
    font-weight: 500;
  }
  .suggestion-chip:hover {
    background: var(--orange);
    border-color: var(--orange);
    color: var(--navy);
  }
 
  .chat-input-area {
    padding: 14px 16px;
    background: white;
    border-top: 1px solid var(--border);
    display: flex;
    gap: 10px;
    align-items: center;
  }
  .chat-input {
    flex-grow: 1;
    border: 1px solid var(--border);
    border-radius: 22px;
    padding: 11px 18px;
    font-size: 14px;
    font-family: inherit;
    resize: none;
    max-height: 100px;
    line-height: 1.4;
    transition: border-color 0.2s;
    outline: none;
  }
  .chat-input:focus { border-color: var(--orange); }
  .chat-send {
    background: var(--orange);
    color: var(--navy);
    border: none;
    width: 42px;
    height: 42px;
    border-radius: 50%;
    cursor: pointer;
    font-size: 18px;
    display: grid;
    place-items: center;
    transition: all 0.2s;
    flex-shrink: 0;
  }
  .chat-send:hover { background: var(--orange-deep); transform: scale(1.05); }
  .chat-send:disabled { opacity: 0.4; cursor: not-allowed; transform: none; }
 
  .typing {
    display: flex;
    gap: 4px;
    padding: 14px 18px;
    background: white;
    border-radius: 14px;
    border-bottom-left-radius: 4px;
    align-self: flex-start;
    box-shadow: 0 2px 8px rgba(15, 28, 48, 0.06);
  }
  .typing span {
    width: 7px; height: 7px;
    background: var(--orange);
    border-radius: 50%;
    animation: typing 1.4s infinite;
  }
  .typing span:nth-child(2) { animation-delay: 0.2s; }
  .typing span:nth-child(3) { animation-delay: 0.4s; }
  @keyframes typing {
    0%, 60%, 100% { opacity: 0.3; transform: translateY(0); }
    30% { opacity: 1; transform: translateY(-4px); }
  }
 
  .chat-disclaimer {
    text-align: center;
    padding: 6px 16px 10px;
    font-size: 10.5px;
    color: var(--text-soft);
    background: white;
  }
 
  @media (max-width: 480px) {
    .chat-panel {
      bottom: 0;
      right: 0;
      left: 0;
      width: 100%;
      max-width: 100%;
      height: 100vh;
      max-height: 100vh;
      border-radius: 0;
    }
    .chat-fab { bottom: 20px; right: 20px; width: 56px; height: 56px; font-size: 24px; }
  }
 
  /* ============ RESPONSIVE ============ */
  @media (max-width: 768px) {
    .nav-links { gap: 16px; }
    .hero { padding: 70px 0 80px; }
    section.block { padding: 60px 0; }
    .quiz-body { padding: 28px 22px; }
    .quiz-header { padding: 22px 24px; }
    .quiz-progress { width: 130px; }
    .matcher-wrap { padding: 24px; }
    .keto-flu-box { grid-template-columns: 1fr; padding: 28px; gap: 28px; }
    .manifesto-grid { grid-template-columns: 1fr; }
    .menu-day { grid-template-columns: 1fr; gap: 6px; }
    .quote-block { padding: 40px 28px; }
    .quote-block blockquote { font-size: 18px; padding-left: 0; }
    .quote-block cite { padding-left: 0; }
  }
</style>
</head>
<body>
 
<nav>
  <div class="container">
    <div class="logo">
      <div class="logo-mark">R</div>
      <span>Raízes · Nutrição Ancestral</span>
    </div>
    <ul class="nav-links">
      <li><a href="#filosofia">Filosofia</a></li>
      <li><a href="#planeador">Planeador</a></li>
      <li><a href="#patologias">Suplementos</a></li>
      <li><a href="#transicao">Transição</a></li>
      <li><a href="#estudos">Estudos</a></li>
      <li><a href="#manifesto">Manifesto</a></li>
    </ul>
  </div>
</nav>
 
<div class="disclaimer-bar">
  <div class="container">
    <strong>Aviso:</strong> Este conteúdo é educativo e não substitui aconselhamento médico. Consulte sempre o seu médico antes de iniciar qualquer dieta ou suplementação, sobretudo se tem patologias diagnosticadas ou toma medicação.
  </div>
</div>
 
<!-- ========== HERO ========== -->
<section class="hero">
  <div class="container">
    <div class="hero-content">
      <span class="hero-tag">Nutrição ancestral · Ciência moderna</span>
      <h1>Volte às <span>raízes</span> do que o corpo humano foi desenhado para comer.</h1>
      <p class="hero-lead">
        Plataforma educativa construída sobre a <strong>evidência científica</strong> acumulada
        em torno das dietas <em>low-carb</em>, cetogénicas e carnívoras. Construa o seu plano
        alimentar, descubra que suplementação é mais adequada ao seu quadro clínico e consulte
        os estudos que sustentam cada recomendação — com base em ciência, não em modas.
      </p>
      <div class="hero-cta">
        <a href="#planeador" class="btn btn-primary">Construir o meu plano</a>
        <a href="#filosofia" class="btn btn-secondary">Compreender primeiro</a>
      </div>
    </div>
  </div>
</section>
 
<!-- ========== FILOSOFIA ========== -->
<section class="block alt" id="filosofia">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Os pilares</div>
      <h2 class="section-title">A doença moderna tem causas modernas.</h2>
      <p class="section-sub">
        Décadas de evidência científica convergem para uma conclusão incómoda: o erro nutricional
        do século XX foi a substituição da gordura natural por hidratos de carbono refinados.
        As consequências estão à vista — diabetes, obesidade, doenças cardiovasculares,
        inflamação crónica como pandemia silenciosa.
      </p>
    </div>
 
    <div class="pillars">
      <div class="pillar">
        <div class="pillar-icon">🌾</div>
        <h3>O verdadeiro vilão é o açúcar</h3>
        <p>Não é a gordura natural que engorda nem entope artérias — é o excesso crónico
        de hidratos de carbono refinados que perpetua a inflamação e a resistência à insulina.</p>
      </div>
      <div class="pillar">
        <div class="pillar-icon">🥩</div>
        <h3>Comida real, densidade nutricional</h3>
        <p>Carnes, peixes, ovos, gorduras saudáveis (manteiga, azeite, banha, coco), vegetais
        de baixo índice glicémico. Sem ultra-processados, sem aditivos, sem óleos vegetais industriais.</p>
      </div>
      <div class="pillar">
        <div class="pillar-icon">🔬</div>
        <h3>Cetose como ferramenta terapêutica</h3>
        <p>Estado metabólico em que o corpo usa corpos cetónicos como combustível. Investigado
        em epilepsia, diabetes, cancro, Alzheimer, Parkinson e doenças autoimunes.</p>
      </div>
      <div class="pillar">
        <div class="pillar-icon">⚖️</div>
        <h3>Jejum intermitente e ritmos</h3>
        <p>Comer menos vezes, mas melhor. Permitir ao corpo períodos de descanso digestivo
        ativa autofagia, regula hormonas e otimiza sensibilidade à insulina.</p>
      </div>
    </div>
 
    <div class="quote-block">
      <blockquote>
        "O homem foi desenhado para comer aquilo que conseguia caçar, pescar ou colher.
        O cereal e o açúcar são invenções recentes na escala evolutiva — e o corpo humano
        ainda não se adaptou a eles."
      </blockquote>
      <cite>— Princípio orientador da nutrição evolutiva</cite>
    </div>
  </div>
</section>
 
<!-- ========== PLANEADOR ========== -->
<section class="block" id="planeador">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Planeador alimentar</div>
      <h2 class="section-title">Que dieta é a certa para si?</h2>
      <p class="section-sub">
        Responda a 5 perguntas curtas. Receberá uma recomendação personalizada — carnívora estrita,
        carnívora-cetogénica, cetogénica clássica, low-carb ou paleo — com princípios e um exemplo
        de menu semanal.
      </p>
    </div>
 
    <div class="quiz-card">
      <div class="quiz-header">
        <h3 id="quiz-title">Pergunta 1 de 5</h3>
        <div class="quiz-progress"><div class="quiz-progress-bar" id="quiz-bar"></div></div>
      </div>
 
      <div class="quiz-body" id="quiz-body">
        <!-- Q1 -->
        <div class="quiz-q active" data-q="1">
          <span class="q-label">Objetivo principal</span>
          <h4>O que pretende alcançar?</h4>
          <div class="options">
            <button class="option" data-val="autoimmune">
              <span class="option-check"></span>
              <span><strong>Reverter / controlar uma patologia</strong> — autoimune, metabólica, inflamatória</span>
            </button>
            <button class="option" data-val="weight">
              <span class="option-check"></span>
              <span><strong>Perder peso e gordura visceral</strong> sem fome nem contagem obsessiva</span>
            </button>
            <button class="option" data-val="energy">
              <span class="option-check"></span>
              <span><strong>Mais energia, foco e clareza mental</strong> ao longo do dia</span>
            </button>
            <button class="option" data-val="performance">
              <span class="option-check"></span>
              <span><strong>Performance física e composição corporal</strong> — treino regular</span>
            </button>
            <button class="option" data-val="longevity">
              <span class="option-check"></span>
              <span><strong>Saúde de longo prazo e longevidade</strong> — prevenção</span>
            </button>
          </div>
        </div>
 
        <!-- Q2 -->
        <div class="quiz-q" data-q="2">
          <span class="q-label">Experiência alimentar</span>
          <h4>Qual é o seu ponto de partida?</h4>
          <div class="options">
            <button class="option" data-val="standard">
              <span class="option-check"></span>
              <span>Dieta ocidental padrão — pão, massas, açúcar presente diariamente</span>
            </button>
            <button class="option" data-val="lowcarb">
              <span class="option-check"></span>
              <span>Já reduzi hidratos antes mas sem grande estrutura</span>
            </button>
            <button class="option" data-val="keto">
              <span class="option-check"></span>
              <span>Já fiz keto ou jejuns prolongados com sucesso</span>
            </button>
            <button class="option" data-val="carnivore">
              <span class="option-check"></span>
              <span>Já experimentei carnívora ou eliminação total de plantas</span>
            </button>
          </div>
        </div>
 
        <!-- Q3 -->
        <div class="quiz-q" data-q="3">
          <span class="q-label">Atividade física</span>
          <h4>Como descreve o seu nível de atividade?</h4>
          <div class="options">
            <button class="option" data-val="sedentary">
              <span class="option-check"></span>
              <span>Sedentário — trabalho de escritório, pouco exercício</span>
            </button>
            <button class="option" data-val="moderate">
              <span class="option-check"></span>
              <span>Moderado — caminho/treino 2 a 4 vezes por semana</span>
            </button>
            <button class="option" data-val="high">
              <span class="option-check"></span>
              <span>Alto — treino intenso 5+ vezes por semana ou desporto competitivo</span>
            </button>
          </div>
        </div>
 
        <!-- Q4 -->
        <div class="quiz-q" data-q="4">
          <span class="q-label">Restrições e sensibilidades</span>
          <h4>Tem alguma destas situações? <em style="color:var(--text-soft); font-size:14px; font-weight:400;">(pode escolher várias)</em></h4>
          <div class="checkbox-grid" id="restrictions">
            <button class="option" data-val="autoimmune">
              <span class="option-check"></span><span>Doença autoimune</span>
            </button>
            <button class="option" data-val="dairy">
              <span class="option-check"></span><span>Intolerância a lácteos</span>
            </button>
            <button class="option" data-val="ibs">
              <span class="option-check"></span><span>Problemas digestivos / SII</span>
            </button>
            <button class="option" data-val="diabetes">
              <span class="option-check"></span><span>Diabetes ou pré-diabetes</span>
            </button>
            <button class="option" data-val="none">
              <span class="option-check"></span><span>Nenhuma das anteriores</span>
            </button>
          </div>
        </div>
 
        <!-- Q5 -->
        <div class="quiz-q" data-q="5">
          <span class="q-label">Estilo de vida</span>
          <h4>Que abordagem se ajusta melhor a si?</h4>
          <div class="options">
            <button class="option" data-val="strict">
              <span class="option-check"></span>
              <span><strong>Quero o protocolo mais limpo possível</strong> — máximo resultado, mesmo que seja restritivo</span>
            </button>
            <button class="option" data-val="balanced">
              <span class="option-check"></span>
              <span><strong>Equilíbrio</strong> — quero variedade e flexibilidade social mantendo princípios</span>
            </button>
            <button class="option" data-val="flexible">
              <span class="option-check"></span>
              <span><strong>Transição suave</strong> — preciso de algo gradual e sustentável</span>
            </button>
          </div>
        </div>
 
        <!-- RESULT -->
        <div class="result-card" id="result">
          <div class="result-banner">
            <span class="badge">Recomendação personalizada</span>
            <h3 id="result-name">—</h3>
            <p id="result-summary">—</p>
          </div>
          <div class="result-body">
            <div class="result-section">
              <h4>Princípios fundamentais</h4>
              <ul class="principles-list" id="result-principles"></ul>
            </div>
            <div class="result-section">
              <h4>Exemplo de menu semanal</h4>
              <div class="menu-week" id="result-menu"></div>
            </div>
            <div class="result-section">
              <h4>Próximo passo</h4>
              <p style="color:var(--text-soft); margin-bottom:18px;">
                Consulte abaixo a secção de <strong>suplementos por patologia</strong> para complementar
                este plano com base no seu quadro clínico, e a secção de <strong>protocolo de transição</strong>
                se ainda não está em cetose.
              </p>
              <button class="btn-action" onclick="document.getElementById('patologias').scrollIntoView({behavior:'smooth'});">
                Ir para suplementos →
              </button>
            </div>
          </div>
        </div>
      </div>
 
      <div class="quiz-footer" id="quiz-footer">
        <button class="btn-quiz btn-quiz-prev" id="btn-prev" disabled>← Anterior</button>
        <button class="btn-quiz btn-quiz-next" id="btn-next" disabled>Seguinte →</button>
      </div>
    </div>
  </div>
</section>
 
<!-- ========== PATOLOGIAS / SUPLEMENTOS ========== -->
<section class="block alt" id="patologias">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Suplementação inteligente</div>
      <h2 class="section-title">Suplementos por patologia, baseados em evidência.</h2>
      <p class="section-sub">
        Selecione as condições que lhe foram diagnosticadas. Cada recomendação inclui dosagens
        de referência publicadas na literatura científica e a base racional do mecanismo. Não substitui
        prescrição médica — serve como ponto de partida para uma conversa informada com o seu profissional de saúde.
      </p>
    </div>
 
    <div class="matcher-wrap">
      <div class="matcher-intro">
        <h3>O seu quadro clínico</h3>
        <p>Selecione uma ou mais patologias diagnosticadas. Pode pesquisar pelo nome.</p>
      </div>
 
      <input type="text" class="pathology-search" id="path-search" placeholder="Pesquisar patologia (ex: diabetes, tiroide, ansiedade...)">
 
      <div class="pathology-grid" id="path-grid"></div>
 
      <div class="matcher-action">
        <button class="btn-action" id="btn-recommend" disabled>Gerar recomendação personalizada</button>
      </div>
 
      <div class="recommendations" id="recommendations"></div>
    </div>
  </div>
</section>
 
<!-- ========== TRANSIÇÃO ========== -->
<section class="block" id="transicao">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Protocolo de transição</div>
      <h2 class="section-title">4 semanas para entrar em cetose com segurança.</h2>
      <p class="section-sub">
        Mudar a fonte de combustível do corpo — de glicose para corpos cetónicos — exige um período
        de adaptação. Este protocolo gradual minimiza desconforto e maximiza a probabilidade de sucesso.
      </p>
    </div>
 
    <div class="transition-grid">
      <div class="week-card">
        <div class="week-header">
          <div class="week-num">Semana 1</div>
          <h4>Eliminar refinados</h4>
        </div>
        <div class="week-body">
          <ul>
            <li>Cortar açúcar adicionado (todas as formas)</li>
            <li>Eliminar farinha branca, pão, bolos</li>
            <li>Adeus refrigerantes e sumos</li>
            <li>Substituir óleos vegetais por azeite, manteiga, banha</li>
            <li>Hidratar bem (2-3L/dia)</li>
          </ul>
        </div>
      </div>
 
      <div class="week-card">
        <div class="week-header">
          <div class="week-num">Semana 2</div>
          <h4>Reduzir hidratos</h4>
        </div>
        <div class="week-body">
          <ul>
            <li>Reduzir para &lt;100g HC/dia</li>
            <li>Eliminar fruta tropical e cereais (mesmo integrais)</li>
            <li>Aumentar gorduras: ovos inteiros, abacate, peixe gordo</li>
            <li>Acrescentar sal de qualidade às refeições</li>
            <li>Iniciar suplementação de magnésio</li>
          </ul>
        </div>
      </div>
 
      <div class="week-card">
        <div class="week-header">
          <div class="week-num">Semana 3</div>
          <h4>Entrar em cetose</h4>
        </div>
        <div class="week-body">
          <ul>
            <li>Reduzir para &lt;30-50g HC/dia</li>
            <li>Apenas vegetais de folha verde e cruciferas</li>
            <li>Proteína moderada (1.2-1.6g/kg)</li>
            <li>Gordura abundante (saciedade)</li>
            <li>Janela alimentar de 8-10h (jejum 14-16h)</li>
          </ul>
        </div>
      </div>
 
      <div class="week-card">
        <div class="week-header">
          <div class="week-num">Semana 4</div>
          <h4>Adaptar e otimizar</h4>
        </div>
        <div class="week-body">
          <ul>
            <li>Cetose estabilizada (medir com tiras urinárias ou ketonix)</li>
            <li>Energia constante, fome regulada</li>
            <li>Avaliar marcadores: glicémia, HOMA-IR, HDL, TG</li>
            <li>Decidir se evoluir para carnívora terapêutica</li>
            <li>Manter ou intensificar jejum intermitente</li>
          </ul>
        </div>
      </div>
    </div>
 
    <div class="keto-flu-box">
      <div>
        <h4>"Keto flu" — o que é e como evitar</h4>
        <p>
          Nos primeiros 7-14 dias é comum sentir cansaço, dor de cabeça, irritabilidade ou cãibras.
          Não é doença — é o corpo a esgotar reservas de glicogénio (que arrastam consigo água e
          eletrólitos). A solução é simples: <strong>repor sódio, potássio e magnésio</strong> de forma agressiva.
        </p>
        <p>
          Bebida caseira: 1 copo de água + ½ colher de chá de <strong>sal marinho não refinado</strong>
          + sumo de meio limão. 1 a 3 vezes por dia até os sintomas desaparecerem.
        </p>
      </div>
      <div>
        <div class="electrolyte-grid">
          <div class="electrolyte">
            <strong>Sódio</strong>
            <span>4-6 g/dia (uma colher de chá de sal de qualidade)</span>
          </div>
          <div class="electrolyte">
            <strong>Potássio</strong>
            <span>3-4 g/dia (abacate, espinafres, salmão)</span>
          </div>
          <div class="electrolyte">
            <strong>Magnésio</strong>
            <span>300-400 mg/dia (glicinato ou citrato)</span>
          </div>
          <div class="electrolyte">
            <strong>Hidratação</strong>
            <span>2-3 L/dia + caldo de osso diário</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
 
<!-- ========== ESTUDOS / REPOSITÓRIO ========== -->
<section class="block alt" id="estudos">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Repositório científico</div>
      <h2 class="section-title">Os estudos que sustentam tudo isto.</h2>
      <p class="section-sub">
        Curadoria dos ensaios clínicos, revisões sistemáticas e meta-análises mais relevantes
        publicados em revistas revistas por pares. Filtre por tema. Cada cartão liga ao artigo
        original em <em>PubMed</em> ou na revista de publicação.
      </p>
    </div>
 
    <div class="studies-filter" id="studies-filter">
      <button class="filter-pill active" data-cat="all">Todos</button>
      <button class="filter-pill" data-cat="diabetes">Diabetes &amp; Metabólico</button>
      <button class="filter-pill" data-cat="cardio">Cardiovascular</button>
      <button class="filter-pill" data-cat="brain">Cérebro &amp; Mental</button>
      <button class="filter-pill" data-cat="autoimmune">Autoimune &amp; Inflamação</button>
      <button class="filter-pill" data-cat="hormonal">Hormonal</button>
      <button class="filter-pill" data-cat="weight">Peso &amp; Composição</button>
      <button class="filter-pill" data-cat="historical">Históricos</button>
    </div>
 
    <div class="studies-grid" id="studies-grid"></div>
 
    <div class="books-row">
      <h3>📚 Livros de referência</h3>
      <div class="books-grid">
        <div class="book">
          <h5>The Art and Science of Low Carbohydrate Living</h5>
          <div class="author">Stephen Phinney &amp; Jeff Volek (2011)</div>
          <p>Manual fundacional para clínicos e pacientes. Explica a fisiologia da cetose e protocolos práticos.</p>
        </div>
        <div class="book">
          <h5>Brain Energy</h5>
          <div class="author">Christopher Palmer, MD (2022)</div>
          <p>Psiquiatra de Harvard apresenta a teoria metabólica das doenças mentais e o uso terapêutico da cetose.</p>
        </div>
        <div class="book">
          <h5>Good Calories, Bad Calories</h5>
          <div class="author">Gary Taubes (2007)</div>
          <p>Investigação histórica e científica que desmonta o paradigma da gordura dietética como vilã.</p>
        </div>
        <div class="book">
          <h5>The Big Fat Surprise</h5>
          <div class="author">Nina Teicholz (2014)</div>
          <p>Análise jornalística rigorosa sobre como ciência fraca capturou guidelines nutricionais.</p>
        </div>
        <div class="book">
          <h5>The Carnivore Code</h5>
          <div class="author">Paul Saladino, MD (2020)</div>
          <p>Argumento científico para o protocolo carnívoro como ferramenta diagnóstica e terapêutica.</p>
        </div>
        <div class="book">
          <h5>The Fat of the Land</h5>
          <div class="author">Vilhjalmur Stefansson (1956)</div>
          <p>Relato pioneiro do explorador que viveu anos exclusivamente de carne com Inuit, sem deficiências.</p>
        </div>
      </div>
    </div>
  </div>
</section>
 
<!-- ========== MANIFESTO PESSOAL ========== -->
<section class="manifesto" id="manifesto">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Manifesto</div>
      <h2 class="section-title">Comer bem é só o princípio.</h2>
    </div>
 
    <div class="manifesto-quote">
      <blockquote>
        "Os homens que querem viver muito quase sempre vivem mal. O que importa não é viver,
        mas viver bem — e viver bem em todos os planos da existência."
      </blockquote>
      <cite>— Adaptado de Fernando Pessoa</cite>
    </div>
 
    <div class="manifesto-grid">
      <div class="manifesto-card">
        <div class="manifesto-avatar">MC</div>
        <h4>Micael Ciência</h4>
        <div class="role">Fundador · Curador deste projeto</div>
        <div class="manifesto-tags">
          <span>Visão holística</span>
          <span>Ciência</span>
          <span>Liberdade</span>
          <span>Propósito</span>
        </div>
        <div class="manifesto-stat">
          <div class="stat-num">∞</div>
          <div class="stat-label">Áreas para otimizar</div>
        </div>
      </div>
 
      <div class="manifesto-text">
        <p>
          Esta plataforma nasce de uma convicção simples: <strong>o corpo é o templo onde
          se constrói tudo o resto</strong> — a clareza para pensar, a energia para trabalhar,
          a paciência para amar, a lucidez para decidir. Reduzir a saúde a calorias e a
          farmácia a remédios é fragmentar aquilo que sempre foi <em class="accent">um todo
          indivisível</em>.
        </p>
        <p>
          A nutrição é apenas o começo. O sono que protegemos, o movimento que praticamos,
          o sol que recebemos, as relações que cultivamos, o trabalho com sentido, a fé que
          nos enraíza — tudo está ligado. Quando uma dimensão sofre, todas adoecem. Quando
          uma floresce, todas se elevam.
        </p>
        <p>
          O meu propósito é simples e demasiado grande para uma só pessoa: <strong>ajudar
          quem cruza o meu caminho a tomar decisões mais lúcidas</strong> em todas as áreas
          que importam — saúde, finanças, trabalho, relações, espírito. Não tenho receitas
          mágicas. Tenho apenas a disciplina de procurar a verdade onde ela está, mesmo
          quando é incómoda, e a coragem de partilhar o que vou aprendendo.
        </p>
        <p>
          Se este site lhe devolveu uma pergunta melhor do que aquela com que chegou —
          então cumpriu o seu papel. <em class="accent">O resto é consigo.</em>
        </p>
      </div>
    </div>
  </div>
</section>
 
<footer>
  <div class="container">
    <p>Construído com rigor por <strong>Micael Ciência</strong> · Fundamentado em literatura científica revista por pares</p>
    <p class="legal">
      Este site tem fins exclusivamente educativos e informativos. As recomendações apresentadas
      baseiam-se em literatura científica disponível, mas não constituem diagnóstico, prescrição
      ou tratamento. Procure sempre acompanhamento médico qualificado antes de iniciar qualquer
      protocolo nutricional ou de suplementação, especialmente se está grávida, a amamentar, toma
      medicação ou tem condições de saúde diagnosticadas.
    </p>
  </div>
</footer>
 
<!-- ========== CHAT ASSISTENTE ========== -->
<button class="chat-fab" id="chat-fab" aria-label="Abrir assistente">💬</button>
<span class="chat-fab-label" id="chat-fab-label">Tem dúvidas? Fale com a Raízes AI</span>
 
<div class="chat-panel" id="chat-panel" role="dialog" aria-label="Assistente Raízes">
  <div class="chat-header">
    <div class="chat-avatar">R</div>
    <div class="chat-info">
      <h4>Raízes AI · Assistente</h4>
      <span>Tira-dúvidas sobre alimentação e suplementação</span>
    </div>
    <button class="chat-close" id="chat-close" aria-label="Fechar">✕</button>
  </div>
 
  <div class="chat-messages" id="chat-messages"></div>
 
  <div class="chat-suggestions" id="chat-suggestions"></div>
 
  <div class="chat-input-area">
    <textarea class="chat-input" id="chat-input" rows="1"
      placeholder="Escreva uma dúvida... (ex: posso comer fruta? tenho enxaqueca)"></textarea>
    <button class="chat-send" id="chat-send" aria-label="Enviar">→</button>
  </div>
 
  <div class="chat-disclaimer">
    Respostas baseadas na base de conhecimento do site. Não substitui aconselhamento médico.
  </div>
</div>
 
<script>
/* ============================================
   QUIZ DE DIETA
   ============================================ */
const quizState = {
  current: 1,
  total: 5,
  answers: {}
};
 
const dietProfiles = {
  carnivora_terapeutica: {
    name: "Carnívora Terapêutica",
    summary: "Protocolo de eliminação total — apenas produtos animais. Indicada para reverter quadros autoimunes, inflamatórios e metabólicos resistentes.",
    principles: [
      "Apenas carne (preferencialmente ruminantes), peixe, ovos, vísceras",
      "Sal de qualidade e água — nada mais nas primeiras 4-8 semanas",
      "Sem lácteos no protocolo inicial (reintroduzir depois se tolerar)",
      "Cortar todos os vegetais, frutas, frutos secos e temperos durante a fase de eliminação",
      "Reintroduzir alimentos um a um após estabilização para identificar gatilhos",
      "Hidratar com caldo de osso diariamente"
    ],
    menu: [
      ["Segunda", "<em>Pequeno-almoço:</em> Ovos com bacon e manteiga<br><em>Almoço:</em> Bife do lombo grelhado, sal grosso<br><em>Jantar:</em> Salmão selvagem em manteiga"],
      ["Terça", "<em>Pequeno-almoço:</em> Jejum (água + sal) ou ovos<br><em>Almoço:</em> Costeletas de borrego<br><em>Jantar:</em> Hambúrguer de vaca caseiro com gema"],
      ["Quarta", "<em>Pequeno-almoço:</em> Ovos mexidos em banha<br><em>Almoço:</em> Fígado de vitela salteado<br><em>Jantar:</em> Sardinhas grelhadas"],
      ["Quinta", "<em>Pequeno-almoço:</em> Caldo de osso<br><em>Almoço:</em> Peito de pato<br><em>Jantar:</em> Costela de vaca lentamente assada"],
      ["Sexta", "<em>Pequeno-almoço:</em> 3 ovos cozidos<br><em>Almoço:</em> Bacalhau fresco com manteiga<br><em>Jantar:</em> Picanha grelhada com sal"],
      ["Sábado", "<em>Pequeno-almoço:</em> Omelete com queijo curado (se tolera)<br><em>Almoço:</em> Coelho estufado<br><em>Jantar:</em> Atum em azeite"],
      ["Domingo", "<em>Pequeno-almoço:</em> Jejum até ao almoço<br><em>Almoço:</em> Cozido familiar (carnes diversas)<br><em>Jantar:</em> Ovos com chouriço de qualidade"]
    ]
  },
  carnivora_keto: {
    name: "Carnívora-Cetogénica",
    summary: "Base animal predominante com pequenas quantidades de vegetais de baixo IG. Excelente equilíbrio entre eficácia terapêutica e flexibilidade.",
    principles: [
      "70-80% das calorias de produtos animais (carne, peixe, ovos, lácteos integrais)",
      "20-30% de gorduras saudáveis: azeite, abacate, frutos secos",
      "Vegetais permitidos: folhas verdes, brócolos, couve-flor, courgette, espargos",
      "Zero açúcar, cereais, leguminosas, óleos vegetais industriais",
      "Janela alimentar de 6-8 horas (jejum 16-18h)",
      "Hidratos &lt; 30g por dia"
    ],
    menu: [
      ["Segunda", "<em>Almoço:</em> Bife com manteiga + salada de espinafres em azeite<br><em>Jantar:</em> Salmão grelhado + brócolos salteados"],
      ["Terça", "<em>Almoço:</em> Omelete de 3 ovos com queijo + abacate<br><em>Jantar:</em> Frango assado com pele + couve-flor"],
      ["Quarta", "<em>Almoço:</em> Salada de atum (azeite, ovo cozido, alface)<br><em>Jantar:</em> Costeletas de borrego + courgette grelhada"],
      ["Quinta", "<em>Almoço:</em> Hambúrguer caseiro sem pão com queijo + bacon<br><em>Jantar:</em> Sardinhas + tomate cherry + azeite"],
      ["Sexta", "<em>Almoço:</em> Bacalhau com natas (sem batata)<br><em>Jantar:</em> Picanha + salada verde"],
      ["Sábado", "<em>Almoço:</em> Polvo com azeite + salada<br><em>Jantar:</em> Entrecôte + espargos com manteiga"],
      ["Domingo", "<em>Almoço:</em> Cozido tradicional (sem batata e arroz)<br><em>Jantar:</em> Ovos mexidos + queijo curado + presunto"]
    ]
  },
  ketogenica: {
    name: "Cetogénica Clássica",
    summary: "Dieta cetogénica equilibrada com variedade de origens. Ideal para perda de peso, controlo metabólico e ganho de energia constante.",
    principles: [
      "Macros aproximados: 70% gordura · 25% proteína · 5% hidratos",
      "Hidratos: máximo 30-50g líquidos por dia",
      "Gorduras de qualidade: azeite extra virgem, abacate, manteiga, coco, ovos, peixe gordo",
      "Proteínas variadas: carne, peixe, ovos, lácteos integrais",
      "Vegetais sem amido à vontade",
      "Frutos vermelhos com moderação (½ chávena/dia)",
      "Jejum intermitente 14-16h opcional mas recomendado"
    ],
    menu: [
      ["Segunda", "<em>Pequeno-almoço:</em> Café bulletproof + 2 ovos<br><em>Almoço:</em> Salada César com frango (sem croutons)<br><em>Jantar:</em> Salmão em manteiga + brócolos"],
      ["Terça", "<em>Pequeno-almoço:</em> Iogurte grego integral + nozes<br><em>Almoço:</em> Bife + salada com abacate<br><em>Jantar:</em> Curgete recheada com carne picada"],
      ["Quarta", "<em>Pequeno-almoço:</em> Omelete com cogumelos e queijo<br><em>Almoço:</em> Sopa de couve-flor + frango<br><em>Jantar:</em> Bacalhau com grão (substituir grão por brócolos)"],
      ["Quinta", "<em>Pequeno-almoço:</em> Jejum<br><em>Almoço:</em> Hambúrguer keto (sem pão) + salada<br><em>Jantar:</em> Sardinhas grelhadas + pimentos assados"],
      ["Sexta", "<em>Pequeno-almoço:</em> 2 ovos + abacate + tomate<br><em>Almoço:</em> Atum + ovo + alface<br><em>Jantar:</em> Frango com pele + espinafres salteados"],
      ["Sábado", "<em>Pequeno-almoço:</em> Panquecas de ovo e queijo<br><em>Almoço:</em> Polvo grelhado + salada<br><em>Jantar:</em> Entrecôte + cogumelos em manteiga"],
      ["Domingo", "<em>Pequeno-almoço:</em> Bowl de iogurte + frutos vermelhos + sementes<br><em>Almoço:</em> Borrego assado + couve-flor gratinada<br><em>Jantar:</em> Tábua de queijos e charcutaria"]
    ]
  },
  lowcarb: {
    name: "Low-Carb Sustentável",
    summary: "Restrição moderada de hidratos com flexibilidade social. Ponto de partida ideal e protocolo manutenção a longo prazo.",
    principles: [
      "Hidratos: 50-100g por dia (privilegiar vegetais e alguma fruta de baixo IG)",
      "Eliminar: açúcar refinado, farinhas brancas, refrigerantes, ultraprocessados",
      "Privilegiar: proteína animal de qualidade, gorduras naturais, vegetais variados",
      "Permitido: bagas (mirtilo, framboesa), maçã, pera com moderação",
      "Sem necessidade de jejum forçado — comer quando tem fome",
      "Manter sempre prioridade da proteína em cada refeição"
    ],
    menu: [
      ["Segunda", "<em>Pequeno-almoço:</em> Ovos + iogurte grego + frutos vermelhos<br><em>Almoço:</em> Frango grelhado + legumes assados<br><em>Jantar:</em> Salmão + salada mista"],
      ["Terça", "<em>Pequeno-almoço:</em> Smoothie de proteína + abacate<br><em>Almoço:</em> Bife + brócolos + ½ chávena de quinoa<br><em>Jantar:</em> Sopa de legumes + omelete"],
      ["Quarta", "<em>Pequeno-almoço:</em> Iogurte + nozes + 1 maçã<br><em>Almoço:</em> Salada de atum com ovo<br><em>Jantar:</em> Frango com cogumelos + courgette"],
      ["Quinta", "<em>Pequeno-almoço:</em> Ovos mexidos + abacate<br><em>Almoço:</em> Sardinhas + salada de tomate<br><em>Jantar:</em> Borrego com legumes assados"],
      ["Sexta", "<em>Pequeno-almoço:</em> Iogurte grego + sementes<br><em>Almoço:</em> Hambúrguer (sem pão) + salada<br><em>Jantar:</em> Bacalhau com legumes"],
      ["Sábado", "<em>Pequeno-almoço:</em> Brunch: ovos + bacon + tomate + abacate<br><em>Almoço:</em> Refeição livre (de preferência peixe ou carne grelhada)<br><em>Jantar:</em> Sopa rica + queijo"],
      ["Domingo", "<em>Pequeno-almoço:</em> Panquecas de aveia (½ porção) + ovos<br><em>Almoço:</em> Almoço familiar — focar em proteína e legumes<br><em>Jantar:</em> Tábua de frios + salada"]
    ]
  },
  paleo: {
    name: "Paleolítica",
    summary: "Alimentação baseada no que conseguíamos caçar, pescar ou colher. Sem cereais, leguminosas ou lácteos, mas com hidratos de raízes e fruta.",
    principles: [
      "Sim: carne, peixe, ovos, vegetais, frutas, frutos secos, sementes, raízes (batata-doce, mandioca)",
      "Não: cereais, leguminosas, lácteos, açúcar refinado, óleos vegetais industriais",
      "Gorduras: azeite, abacate, coco, manteiga clarificada (ghee), banha",
      "Mais permissiva em hidratos do que keto — boa para atletas",
      "Foco em qualidade: orgânico, pasto, selvagem quando possível",
      "Hidratos a girar em torno do treino"
    ],
    menu: [
      ["Segunda", "<em>Pequeno-almoço:</em> Ovos + abacate + frutos vermelhos<br><em>Almoço:</em> Frango + batata-doce assada + brócolos<br><em>Jantar:</em> Salmão + espargos"],
      ["Terça", "<em>Pequeno-almoço:</em> Smoothie verde + frutos secos<br><em>Almoço:</em> Bife + salada + ½ batata-doce<br><em>Jantar:</em> Sopa de cenoura + frango assado"],
      ["Quarta", "<em>Pequeno-almoço:</em> Omelete com legumes<br><em>Almoço:</em> Salada de atum com azeite e abacate<br><em>Jantar:</em> Costeletas de borrego + couve-flor"],
      ["Quinta", "<em>Pequeno-almoço:</em> Banana + amêndoas + 2 ovos<br><em>Almoço:</em> Hambúrguer (sem pão) + batata-doce frita em azeite<br><em>Jantar:</em> Sardinhas + tomate"],
      ["Sexta", "<em>Pequeno-almoço:</em> Bowl de frutos vermelhos + sementes<br><em>Almoço:</em> Frango com legumes salteados<br><em>Jantar:</em> Polvo + salada"],
      ["Sábado", "<em>Pequeno-almoço:</em> Ovos + bacon + cogumelos<br><em>Almoço:</em> Carne assada + raízes assadas<br><em>Jantar:</em> Peixe com legumes ao vapor"],
      ["Domingo", "<em>Pequeno-almoço:</em> Panquecas de banana e ovo<br><em>Almoço:</em> Cozido (sem grão e arroz) + couves<br><em>Jantar:</em> Salada completa + ovo cozido"]
    ]
  }
};
 
function decideDiet() {
  const a = quizState.answers;
  const restrictions = a[4] || [];
  const isAutoimmune = restrictions.includes("autoimmune") || a[1] === "autoimmune";
  const isStrict = a[5] === "strict";
  const isFlexible = a[5] === "flexible";
  const experienced = a[2] === "carnivore" || a[2] === "keto";
 
  // Carnívora terapêutica: autoimune + strict + experiência
  if (isAutoimmune && isStrict) return "carnivora_terapeutica";
  if (isAutoimmune && experienced) return "carnivora_keto";
 
  // Diabetes/metabólico
  if (restrictions.includes("diabetes") && isStrict) return "carnivora_keto";
  if (restrictions.includes("diabetes")) return "ketogenica";
 
  // Performance + experiência
  if (a[1] === "performance" && a[3] === "high") return "paleo";
 
  // Energia + clareza mental
  if (a[1] === "energy" && !isFlexible) return "ketogenica";
 
  // Iniciante / transição suave
  if (a[2] === "standard" && isFlexible) return "lowcarb";
  if (isFlexible) return "lowcarb";
 
  // Strict generic
  if (isStrict && experienced) return "carnivora_keto";
  if (isStrict) return "ketogenica";
 
  // Default
  if (a[1] === "longevity") return "paleo";
  if (a[1] === "weight") return "ketogenica";
 
  return "lowcarb";
}
 
function showResult() {
  const dietKey = decideDiet();
  const diet = dietProfiles[dietKey];
 
  document.getElementById("result-name").textContent = diet.name;
  document.getElementById("result-summary").textContent = diet.summary;
 
  const ul = document.getElementById("result-principles");
  ul.innerHTML = diet.principles.map(p => `<li>${p}</li>`).join("");
 
  const menu = document.getElementById("result-menu");
  menu.innerHTML = diet.menu.map(([day, meals]) =>
    `<div class="menu-day"><strong>${day}</strong><div class="menu-meals">${meals}</div></div>`
  ).join("");
 
  document.querySelectorAll(".quiz-q").forEach(q => q.classList.remove("active"));
  document.getElementById("result").classList.add("active");
  document.getElementById("quiz-title").textContent = "A sua recomendação";
  document.getElementById("quiz-bar").style.width = "100%";
  document.getElementById("quiz-footer").style.display = "none";
}
 
// Quiz interaction
document.querySelectorAll(".quiz-q").forEach(q => {
  const qNum = parseInt(q.dataset.q);
  const isMulti = q.querySelector(".checkbox-grid") !== null;
 
  q.querySelectorAll(".option").forEach(btn => {
    btn.addEventListener("click", () => {
      if (isMulti) {
        // Multi-select: handle "none" as exclusive
        if (btn.dataset.val === "none") {
          q.querySelectorAll(".option").forEach(b => b.classList.remove("selected"));
          btn.classList.add("selected");
        } else {
          q.querySelector('[data-val="none"]')?.classList.remove("selected");
          btn.classList.toggle("selected");
        }
        const selected = Array.from(q.querySelectorAll(".option.selected")).map(b => b.dataset.val);
        quizState.answers[qNum] = selected.filter(v => v !== "none");
        document.getElementById("btn-next").disabled = selected.length === 0;
      } else {
        q.querySelectorAll(".option").forEach(b => b.classList.remove("selected"));
        btn.classList.add("selected");
        quizState.answers[qNum] = btn.dataset.val;
        document.getElementById("btn-next").disabled = false;
      }
    });
  });
});
 
document.getElementById("btn-next").addEventListener("click", () => {
  if (quizState.current === quizState.total) {
    showResult();
    return;
  }
  document.querySelector(`.quiz-q[data-q="${quizState.current}"]`).classList.remove("active");
  quizState.current++;
  document.querySelector(`.quiz-q[data-q="${quizState.current}"]`).classList.add("active");
  document.getElementById("quiz-title").textContent = `Pergunta ${quizState.current} de ${quizState.total}`;
  document.getElementById("quiz-bar").style.width = (quizState.current / quizState.total * 100) + "%";
  document.getElementById("btn-prev").disabled = false;
  document.getElementById("btn-next").textContent = quizState.current === quizState.total ? "Ver recomendação →" : "Seguinte →";
 
  const currentQ = document.querySelector(`.quiz-q[data-q="${quizState.current}"]`);
  const isMulti = currentQ.querySelector(".checkbox-grid") !== null;
  if (isMulti) {
    document.getElementById("btn-next").disabled = !(quizState.answers[quizState.current]?.length > 0);
  } else {
    document.getElementById("btn-next").disabled = !quizState.answers[quizState.current];
  }
});
 
document.getElementById("btn-prev").addEventListener("click", () => {
  if (quizState.current === 1) return;
  document.querySelector(`.quiz-q[data-q="${quizState.current}"]`).classList.remove("active");
  quizState.current--;
  document.querySelector(`.quiz-q[data-q="${quizState.current}"]`).classList.add("active");
  document.getElementById("quiz-title").textContent = `Pergunta ${quizState.current} de ${quizState.total}`;
  document.getElementById("quiz-bar").style.width = (quizState.current / quizState.total * 100) + "%";
  document.getElementById("btn-prev").disabled = quizState.current === 1;
  document.getElementById("btn-next").textContent = "Seguinte →";
  document.getElementById("btn-next").disabled = false;
});
 
/* ============================================
   PATOLOGIA → SUPLEMENTOS
   ============================================ */
const pathologies = {
  diabetes: {
    name: "Diabetes Tipo 2 / Resistência à Insulina",
    diet: "Cetogénica ou Carnívora-Keto",
    rationale: "A restrição de hidratos é a intervenção mais eficaz documentada para reverter a resistência à insulina (Westman et al., 2008; Hallberg et al., 2018 — estudo Virta Health a 2 anos). A cetose nutricional baixa rapidamente glicémia e HOMA-IR, frequentemente eliminando necessidade de medicação.",
    supplements: [
      ["Magnésio (glicinato/citrato)", "300-400 mg/dia", "Cofator essencial na sinalização da insulina; deficiência prevalente em diabéticos."],
      ["Berberina", "500 mg, 2-3x/dia", "Eficácia comparável à metformina em vários ensaios (Yin et al., 2008). Ativa AMPK."],
      ["Vitamina D3", "2000-5000 UI/dia", "Níveis baixos correlacionam com pior controlo glicémico (Pittas et al., 2007)."],
      ["Ómega-3 (EPA+DHA)", "2-3 g/dia", "Reduz inflamação, melhora perfil lipídico e sensibilidade à insulina."],
      ["Crómio (picolinato)", "200-400 mcg/dia", "Potencia ação da insulina nos recetores celulares."],
      ["Ácido alfa-lipóico", "300-600 mg/dia", "Antioxidante; estudos mostram melhoria da neuropatia diabética."]
    ]
  },
  hypertension: {
    name: "Hipertensão Arterial",
    diet: "Cetogénica ou Low-Carb com sal de qualidade",
    rationale: "Contrariando o dogma, a restrição de hidratos baixa a tensão arterial mais eficazmente do que a restrição de sal (Volek et al.). A hiperinsulinémia crónica é causa central de hipertensão essencial.",
    supplements: [
      ["Magnésio", "400-600 mg/dia", "Vasodilatador natural. Meta-análises mostram redução média de 3-4 mmHg (Zhang et al., 2016)."],
      ["Coenzima Q10", "100-200 mg/dia", "Reduz tensão sistólica em 11-17 mmHg em estudos clínicos (Rosenfeldt et al., 2007)."],
      ["Ómega-3", "2-4 g/dia", "Reduz tensão e melhora função endotelial."],
      ["Potássio (alimentar)", "3-4 g/dia", "Abacate, espinafres, salmão. Antagonista natural do sódio."],
      ["Beterraba (nitratos)", "250 ml sumo/dia", "Donadores de óxido nítrico — vasodilatação."],
      ["L-Arginina / Citrulina", "3-6 g/dia", "Precursores de óxido nítrico."]
    ]
  },
  metabolic: {
    name: "Síndrome Metabólica",
    diet: "Cetogénica estrita",
    rationale: "Síndrome metabólica = manifestação da hiperinsulinémia crónica. A restrição severa de hidratos resolve simultaneamente as 5 componentes (perímetro abdominal, triglicéridos, HDL baixo, HTA, glicémia jejum).",
    supplements: [
      ["Berberina", "500 mg, 2-3x/dia", "Atua em múltiplas vias metabólicas — glicose, lípidos, peso."],
      ["Magnésio", "400 mg/dia", "Deficiência presente em >75% dos casos."],
      ["Ómega-3", "2-3 g/dia", "Baixa triglicéridos significativamente."],
      ["Vitamina D3 + K2", "5000 UI + 100 mcg/dia", "Modula inflamação sistémica."],
      ["Ácido alfa-lipóico", "600 mg/dia", "Melhora sensibilidade insulina e perfil lipídico."],
      ["Inositol (Myo-inositol)", "2-4 g/dia", "Particularmente eficaz em mulheres com componente hormonal."]
    ]
  },
  nafld: {
    name: "Esteatose Hepática (Fígado Gordo)",
    diet: "Cetogénica — primeira linha",
    rationale: "A esteatose hepática não-alcoólica é causada por excesso de frutose e hidratos refinados. Estudos (Browning et al., 2011) mostram redução de 55% da gordura hepática em apenas 2 semanas de dieta cetogénica.",
    supplements: [
      ["Colina", "500-1000 mg/dia", "Essencial para exportação hepática de gordura. Deficiência causa esteatose."],
      ["Inositol", "2-4 g/dia", "Cofator lipotrópico, mobiliza gordura hepática."],
      ["NAC (N-acetilcisteína)", "600-1200 mg/dia", "Precursor de glutationa, principal antioxidante hepático."],
      ["Vitamina E (tocoferóis mistos)", "400-800 UI/dia", "Recomendada por guidelines AASLD para NAFLD."],
      ["Cardo Mariano (Silimarina)", "200-400 mg/dia", "Hepatoprotetor com séculos de uso clínico."],
      ["Ómega-3", "3-4 g/dia", "Reduz triglicéridos hepáticos."]
    ]
  },
  cholesterol: {
    name: "Dislipidémia (Colesterol/Triglicéridos)",
    diet: "Cetogénica ou Carnívora-Keto",
    rationale: "Triglicéridos altos e HDL baixo são consequência de excesso de hidratos, não de gordura. Dietas low-carb baixam TG drasticamente e elevam HDL. O LDL pode subir mas geralmente em padrão A (partículas grandes, não aterogénicas).",
    supplements: [
      ["Ómega-3 (EPA)", "2-4 g/dia", "Reduz triglicéridos em 20-50% (icosapent ethyl em REDUCE-IT)."],
      ["Levedura de arroz vermelho", "1200-2400 mg/dia", "Contém monacolina K (lovastatina natural) — eficaz e melhor tolerado."],
      ["CoQ10", "100-200 mg/dia", "Essencial se toma estatinas (deplecionam CoQ10)."],
      ["Niacina (B3)", "500-1000 mg/dia", "Eleva HDL eficazmente; cuidado com flush."],
      ["Bergamota (extrato)", "500-1000 mg/dia", "Reduz LDL e melhora HDL em ensaios clínicos italianos."],
      ["Psyllium (fibra solúvel)", "5-10 g/dia", "Sequestra ácidos biliares, baixa LDL."]
    ]
  },
  hypothyroid: {
    name: "Hipotiroidismo (incluindo Hashimoto)",
    diet: "Carnívora-Keto ou Paleo (AIP se autoimune)",
    rationale: "Hashimoto é a causa mais comum de hipotiroidismo no Ocidente. A eliminação de glúten e a redução de inflamação intestinal são fundamentais. A cetose pode reduzir a necessidade de medicação ao longo do tempo.",
    supplements: [
      ["Selénio (selenometionina)", "200 mcg/dia", "Reduz anticorpos TPO em Hashimoto (Toulis et al., 2010). 2 castanhas do Brasil/dia."],
      ["Zinco", "15-30 mg/dia", "Cofator na conversão T4→T3."],
      ["Iodo", "150-300 mcg/dia", "Cuidado com dosagens altas em Hashimoto — preferir alimentar (ovos, peixe)."],
      ["Vitamina D3", "5000 UI/dia", "Imunomodulador essencial em autoimunes."],
      ["L-Tirosina", "500-1500 mg/dia", "Aminoácido precursor das hormonas tiroideias."],
      ["Magnésio", "400 mg/dia", "Cofator em mais de 300 enzimas, frequentemente baixo."]
    ]
  },
  autoimmune: {
    name: "Doenças Autoimunes (Lúpus, AR, Esclerose Múltipla)",
    diet: "Carnívora terapêutica ou Cetogénica AIP",
    rationale: "A permeabilidade intestinal ('leaky gut') é fator central na patogénese autoimune. Eliminar todos os potenciais gatilhos (cereais, leguminosas, lácteos, plantas com lectinas/oxalatos) durante 60-90 dias permite reset imunitário documentado em vários ensaios clínicos.",
    supplements: [
      ["Vitamina D3 + K2", "5000-10000 UI + 200 mcg/dia", "Imunomodulador crítico — alvo: 50-80 ng/mL no sangue."],
      ["Ómega-3 (EPA)", "3-4 g/dia", "Anti-inflamatório sistémico."],
      ["Curcumina (com piperina)", "500-1000 mg/dia", "Inibidor potente de NF-κB."],
      ["L-Glutamina", "5-15 g/dia", "Combustível dos enterócitos; restaura barreira intestinal."],
      ["Probióticos multi-estirpe", "20-50 bilhões UFC/dia", "Modulação da microbiota e tolerância imunitária."],
      ["LDN (Naltrexona Baixa Dose)", "Prescrição médica", "Modulador imunitário cada vez mais usado em autoimunes."]
    ]
  },
  pcos: {
    name: "Síndrome do Ovário Poliquístico (SOP)",
    diet: "Cetogénica — primeira linha",
    rationale: "SOP é fundamentalmente um distúrbio de resistência à insulina. A restrição de hidratos restaura ovulação, baixa testosterona livre, melhora acne e regularidade menstrual. Estudos com inositol mostram eficácia comparável à metformina.",
    supplements: [
      ["Inositol (Myo+D-Chiro 40:1)", "4 g + 100 mg/dia", "Restaura sensibilidade insulina ovárica e ovulação (Unfer et al., 2017)."],
      ["Vitamina D3", "4000-5000 UI/dia", "Deficiência muito prevalente em SOP."],
      ["NAC", "600 mg, 2x/dia", "Comparável à metformina em melhorar ovulação (Thakker et al., 2015)."],
      ["Ómega-3", "2-3 g/dia", "Reduz testosterona, melhora ciclo."],
      ["Magnésio", "400 mg/dia", "Sensibilidade insulina + sintomas pré-menstruais."],
      ["Berberina", "500 mg, 3x/dia", "Eficaz em SOP com componente metabólica forte."]
    ]
  },
  depression: {
    name: "Depressão / Ansiedade",
    diet: "Cetogénica — investigação muito promissora",
    rationale: "A 'Metabolic Psychiatry' (Dr. Chris Palmer, Harvard) defende as doenças mentais como problemas metabólicos cerebrais. Os corpos cetónicos são neuroprotetores. Estudos pilotos em depressão refratária com keto mostram resultados notáveis.",
    supplements: [
      ["Ómega-3 (EPA >60%)", "1-2 g EPA/dia", "Meta-análises mostram efeito antidepressivo equivalente a SSRIs em alguns subgrupos."],
      ["Vitamina D3", "4000-5000 UI/dia", "Deficiência fortemente associada a depressão sazonal e major."],
      ["Magnésio (glicinato/treonato)", "400 mg/dia", "Treonato atravessa barreira hematoencefálica; evidência crescente."],
      ["B12 (metilcobalamina) + Folato", "1000 mcg + 400 mcg/dia", "Cofatores na síntese de neurotransmissores."],
      ["L-Triptofano ou 5-HTP", "100-300 mg à noite", "Precursores de serotonina. NÃO combinar com SSRIs."],
      ["SAMe", "400-800 mg/dia", "Doador de metilo; eficácia comparável a tricíclicos em alguns estudos."]
    ]
  },
  insomnia: {
    name: "Insónia / Distúrbios do Sono",
    diet: "Low-Carb ou Cetogénica",
    rationale: "Excesso de hidratos refinados e estimulantes desregulam ciclos circadianos. A cetose estabiliza glicémia noturna e melhora arquitetura do sono em muitos protocolos.",
    supplements: [
      ["Magnésio (glicinato)", "400 mg, 1h antes de deitar", "Relaxa SNC e musculatura."],
      ["Glicina", "3 g antes de deitar", "Baixa temperatura corporal central, melhora sono profundo."],
      ["L-Teanina", "200-400 mg", "Promove ondas alfa (relaxamento sem sedação)."],
      ["Melatonina", "0.3-1 mg (NÃO 5-10mg)", "Doses fisiológicas são mais eficazes que altas; usar 30 min antes de deitar."],
      ["Apigenina (camomila)", "50 mg", "GABAérgico suave."],
      ["Ashwagandha", "300-600 mg/dia", "Adaptogénico; reduz cortisol em pessoas com stress crónico."]
    ]
  },
  migraine: {
    name: "Enxaqueca",
    diet: "Cetogénica — primeira linha terapêutica",
    rationale: "A dieta cetogénica foi originalmente desenvolvida para epilepsia e mostra eficácia notável em enxaqueca crónica. Estudos (Di Lorenzo et al., 2015) mostram redução de 80% na frequência em ensaios clínicos.",
    supplements: [
      ["Magnésio (glicinato)", "400-600 mg/dia", "Recomendado por guidelines da American Headache Society."],
      ["Riboflavina (B2)", "400 mg/dia", "Melhora função mitocondrial; reduz frequência em ~50%."],
      ["CoQ10", "100 mg, 3x/dia", "Estudo placebo-controlado mostrou redução significativa da frequência."],
      ["Ómega-3", "2-3 g/dia", "Anti-inflamatório."],
      ["Tanaceto (Feverfew)", "100-300 mg/dia", "Profilaxia tradicional com evidência."],
      ["Petasites (Butterbur)", "75 mg, 2x/dia", "Eficácia comparável a topiramato em alguns estudos."]
    ]
  },
  ibs: {
    name: "Síndrome do Intestino Irritável / SIBO",
    diet: "Carnívora terapêutica (para SIBO severo) ou Cetogénica baixa em FODMAPs",
    rationale: "A eliminação de fibras fermentáveis e amidos resistentes 'mata à fome' o sobrecrescimento bacteriano. A dieta carnívora é frequentemente curativa em casos severos. Reintroduzir gradualmente após estabilização.",
    supplements: [
      ["L-Glutamina", "5-15 g/dia em jejum", "Combustível principal dos enterócitos; restaura barreira intestinal."],
      ["Probióticos (S. boulardii)", "5-10 bilhões/dia", "Levedura probiótica resistente a antibióticos."],
      ["Hortelã-pimenta (cápsulas entéricas)", "200-400 mg, 3x/dia", "Antiespasmódico — guidelines do American College of Gastroenterology."],
      ["Berberina", "500 mg, 3x/dia", "Antimicrobiano natural eficaz em SIBO."],
      ["Enzimas digestivas", "Com refeições", "Ajudam digestão durante fase aguda."],
      ["Zinco-carnosina", "75 mg, 2x/dia", "Cicatrizante da mucosa gástrica e intestinal."]
    ]
  },
  reflux: {
    name: "Refluxo Gastroesofágico (DRGE)",
    diet: "Low-Carb ou Cetogénica",
    rationale: "Contrariando a abordagem convencional, o refluxo está mais associado a HIPOclorídria (ácido a menos) do que hiperclorídria. A redução de hidratos baixa pressão intra-abdominal e refluxo (Austin et al., 2006).",
    supplements: [
      ["Betaína HCl + Pepsina", "500-1500 mg com refeições proteicas", "Restaura acidez gástrica fisiológica."],
      ["DGL (alcaçuz desglicirrizinado)", "400 mg antes das refeições", "Cicatrizante da mucosa esofágica e gástrica."],
      ["Enzimas digestivas (com lipase)", "Com refeições", "Apoia digestão gastrelímpia."],
      ["Aloe vera (interno)", "30 ml antes das refeições", "Calmante da mucosa."],
      ["L-Glutamina", "5 g/dia", "Reparação tecidular."],
      ["Melatonina (noite)", "3-6 mg", "Demonstrada redução de DRGE em ensaios clínicos (Kandil et al., 2010)."]
    ]
  },
  osteoporosis: {
    name: "Osteoporose / Osteopenia",
    diet: "Carnívora-Keto ou Paleo rica em proteína",
    rationale: "A osteoporose não é primariamente défice de cálcio — é défice de matriz proteica e vitaminas K2/D3. Dietas ricas em proteína animal aumentam densidade óssea (contrariando o mito da 'acidose'). Treino de força é essencial.",
    supplements: [
      ["Vitamina D3", "5000-10000 UI/dia", "Alvo: 50-70 ng/mL. Sem D3 não há absorção de cálcio."],
      ["Vitamina K2 (MK-7)", "180-360 mcg/dia", "Direciona cálcio para osso (não para artérias). Crítico."],
      ["Magnésio", "400-600 mg/dia", "Cofator essencial; 50% do magnésio do corpo está nos ossos."],
      ["Cálcio (alimentar > suplemento)", "1000-1200 mg/dia", "Preferir lácteos integrais, sardinhas, vegetais verdes."],
      ["Boro", "3-10 mg/dia", "Reduz perda urinária de cálcio e magnésio."],
      ["Colagénio hidrolisado", "10-20 g/dia", "Matriz óssea é 90% colagénio."]
    ]
  },
  fatigue: {
    name: "Fadiga Crónica / Burnout",
    diet: "Cetogénica com refeições densas em nutrientes",
    rationale: "A fadiga crónica reflete frequentemente disfunção mitocondrial e desregulação do eixo HPA (cortisol). A cetose providencia combustível mitocondrial mais eficiente (corpos cetónicos > glicose).",
    supplements: [
      ["B12 (metilcobalamina)", "1000-5000 mcg/dia", "Deficiência subclínica é endémica."],
      ["Ferro (se ferritina baixa)", "Conforme análises", "NUNCA suplementar sem confirmar deficiência."],
      ["CoQ10 (ubiquinol)", "200-400 mg/dia", "Combustível mitocondrial direto."],
      ["D-Ribose", "5 g, 3x/dia", "Substrato para ATP — utilizada em fibromialgia e síndrome fadiga crónica."],
      ["Adaptogénios (Rhodiola, Ashwagandha)", "300-500 mg/dia", "Modulam resposta ao stress."],
      ["Magnésio + Complexo B", "400 mg + B-complex/dia", "Cofatores para produção energética."]
    ]
  },
  inflammation: {
    name: "Inflamação Crónica / Artrite",
    diet: "Carnívora-Keto ou Cetogénica AIP",
    rationale: "A inflamação crónica de baixo grau está na raiz de praticamente todas as doenças degenerativas. A cetose reduz inflamação por múltiplos mecanismos: BHB inibe NLRP3 inflamassoma, reduz espécies reativas, melhora função mitocondrial.",
    supplements: [
      ["Curcumina (com piperina ou nano)", "500-1000 mg, 2x/dia", "Eficácia comparável a AINEs em ensaios de osteoartrite."],
      ["Ómega-3 (EPA+DHA)", "3-4 g/dia", "Precursor de mediadores anti-inflamatórios (resolvinas, protetinas)."],
      ["Boswellia serrata", "300-500 mg, 2-3x/dia", "Inibidor de 5-LOX; estudos clínicos em artrite e Crohn."],
      ["Glucosamina + Condroitina", "1500 mg + 1200 mg/dia", "Estudo GAIT; eficaz em casos moderados a severos."],
      ["MSM (metilsulfonilmetano)", "3-6 g/dia", "Reduz dor e rigidez em estudos clínicos."],
      ["Vitamina D3 + K2", "5000 UI + 100 mcg/dia", "Imunomodulador sistémico."]
    ]
  }
};
 
// Render pathology grid
const grid = document.getElementById("path-grid");
Object.entries(pathologies).forEach(([key, data]) => {
  const btn = document.createElement("button");
  btn.className = "pathology-chip";
  btn.dataset.key = key;
  btn.innerHTML = `<span class="chip-check"></span><span>${data.name.split(" / ")[0].split(" (")[0]}</span>`;
  btn.addEventListener("click", () => {
    btn.classList.toggle("selected");
    const anySelected = document.querySelectorAll(".pathology-chip.selected").length > 0;
    document.getElementById("btn-recommend").disabled = !anySelected;
  });
  grid.appendChild(btn);
});
 
// Search filter
document.getElementById("path-search").addEventListener("input", (e) => {
  const term = e.target.value.toLowerCase();
  document.querySelectorAll(".pathology-chip").forEach(chip => {
    const matches = pathologies[chip.dataset.key].name.toLowerCase().includes(term);
    chip.style.display = matches ? "" : "none";
  });
});
 
// Generate recommendations
document.getElementById("btn-recommend").addEventListener("click", () => {
  const selected = Array.from(document.querySelectorAll(".pathology-chip.selected"))
    .map(c => c.dataset.key);
  const recDiv = document.getElementById("recommendations");
 
  recDiv.innerHTML = `
    <div style="background:#fff8e7; border:1px solid #f0deaa; padding:18px 22px; border-radius:10px; margin-bottom:24px; font-size:14px; color:#6b5618;">
      <strong>⚠ Importante:</strong> As doses indicadas são valores de referência da literatura científica.
      Devem ser ajustadas individualmente por profissional de saúde, especialmente se toma medicação
      crónica ou tem condições hepáticas/renais. Comece sempre na dose mais baixa.
    </div>
  ` + selected.map(key => {
    const p = pathologies[key];
    const rows = p.supplements.map(([name, dose, why]) =>
      `<tr><td>${name}</td><td>${dose}</td><td>${why}</td></tr>`
    ).join("");
    return `
      <div class="rec-card">
        <h4>${p.name}</h4>
        <div class="rec-diet">Dieta recomendada: ${p.diet}</div>
        <p class="rec-rationale"><strong>Base científica:</strong> ${p.rationale}</p>
        <table class="supplements-table">
          <thead>
            <tr><th>Suplemento</th><th>Dose de referência</th><th>Mecanismo / Evidência</th></tr>
          </thead>
          <tbody>${rows}</tbody>
        </table>
      </div>
    `;
  }).join("");
 
  recDiv.classList.add("active");
  setTimeout(() => recDiv.scrollIntoView({behavior:"smooth", block:"start"}), 100);
});
 
/* ============================================
   REPOSITÓRIO DE ESTUDOS
   ============================================ */
const studies = [
  // ===== DIABETES & METABÓLICO =====
  {
    cat: "diabetes",
    tag: "Ensaio clínico · 2 anos",
    title: "Effectiveness and Safety of a Novel Care Model for the Management of Type 2 Diabetes at 1 Year",
    authors: "Hallberg SJ, et al. (Virta Health)",
    journal: "Diabetes Therapy, 2018",
    finding: "Em 262 adultos com DT2, intervenção de cetose nutricional reduziu HbA1c de 7.6% para 6.3% e permitiu eliminar ou reduzir medicação em <strong>94%</strong> dos pacientes que tomavam insulina. Resultados sustentados a 2 anos.",
    url: "https://link.springer.com/article/10.1007/s13300-018-0373-9"
  },
  {
    cat: "diabetes",
    tag: "Ensaio clínico",
    title: "The effect of a low-carbohydrate, ketogenic diet versus a low-glycemic index diet on glycemic control in type 2 diabetes mellitus",
    authors: "Westman EC, et al.",
    journal: "Nutrition &amp; Metabolism, 2008",
    finding: "Dieta cetogénica (&lt;20g HC/dia) superou significativamente dieta de baixo IG na redução de HbA1c, peso e necessidade de medicação em diabéticos tipo 2 ao longo de 24 semanas.",
    url: "https://nutritionandmetabolism.biomedcentral.com/articles/10.1186/1743-7075-5-36"
  },
  {
    cat: "diabetes",
    tag: "Meta-análise",
    title: "Efficacy and safety of low and very low carbohydrate diets for type 2 diabetes remission",
    authors: "Goldenberg JZ, et al.",
    journal: "BMJ, 2021",
    finding: "Revisão sistemática de 23 ensaios (1357 pacientes): dietas low-carb a 6 meses produziram remissão de DT2 em <strong>57%</strong> dos pacientes vs 31% em controlo, com perda de peso e melhoria em todos os marcadores metabólicos.",
    url: "https://www.bmj.com/content/372/bmj.m4743"
  },
  {
    cat: "diabetes",
    tag: "Estudo Counterpoint",
    title: "Reversal of type 2 diabetes: normalisation of beta cell function in association with decreased pancreas and liver triacylglycerol",
    authors: "Lim EL, et al.",
    journal: "Diabetologia, 2011",
    finding: "Estudo seminal demonstrou que DT2 é reversível através da remoção de gordura ectópica do pâncreas e fígado. Função das células beta normalizou em 8 semanas. Base científica para o paradigma da reversão.",
    url: "https://link.springer.com/article/10.1007/s00125-011-2204-7"
  },
  {
    cat: "diabetes",
    tag: "Berberina vs Metformina",
    title: "Efficacy of berberine in patients with type 2 diabetes mellitus",
    authors: "Yin J, Xing H, Ye J",
    journal: "Metabolism, 2008",
    finding: "Berberina 500mg 3x/dia reduziu HbA1c, glicémia em jejum e pós-prandial de forma comparável à metformina, com adicional melhoria do perfil lipídico (TG -35%, colesterol total -29%).",
    url: "https://pubmed.ncbi.nlm.nih.gov/18397984/"
  },
 
  // ===== CARDIOVASCULAR =====
  {
    cat: "cardio",
    tag: "Ensaio DIRECT · 2 anos",
    title: "Weight Loss with a Low-Carbohydrate, Mediterranean, or Low-Fat Diet",
    authors: "Shai I, et al.",
    journal: "New England Journal of Medicine, 2008",
    finding: "Comparação a 2 anos entre 3 dietas em 322 participantes: low-carb produziu maior perda de peso e <strong>melhor perfil lipídico</strong> (HDL, TG) que dieta low-fat — desafiando o consenso vigente.",
    url: "https://www.nejm.org/doi/full/10.1056/NEJMoa0708681"
  },
  {
    cat: "cardio",
    tag: "Ensaio REDUCE-IT",
    title: "Cardiovascular Risk Reduction with Icosapent Ethyl for Hypertriglyceridemia",
    authors: "Bhatt DL, et al.",
    journal: "New England Journal of Medicine, 2019",
    finding: "8.179 pacientes com TG elevados em prevenção secundária: 4g EPA reduziu eventos cardiovasculares em <strong>25%</strong> ao longo de 4.9 anos. Efeito independente da redução de TG.",
    url: "https://www.nejm.org/doi/full/10.1056/NEJMoa1812792"
  },
  {
    cat: "cardio",
    tag: "Meta-análise",
    title: "Effects of magnesium supplementation on blood pressure: a meta-analysis",
    authors: "Zhang X, et al.",
    journal: "Hypertension, 2016",
    finding: "Análise de 34 ensaios randomizados controlados: suplementação de magnésio (mediana 368 mg/dia, 3 meses) reduziu tensão sistólica em 2.00 mmHg e diastólica em 1.78 mmHg.",
    url: "https://www.ahajournals.org/doi/10.1161/HYPERTENSIONAHA.116.07664"
  },
  {
    cat: "cardio",
    tag: "Ensaio clínico",
    title: "Coenzyme Q10 in the treatment of hypertension: a meta-analysis",
    authors: "Rosenfeldt FL, et al.",
    journal: "Journal of Human Hypertension, 2007",
    finding: "Meta-análise de 12 ensaios mostrou que CoQ10 reduziu tensão sistólica em até <strong>17 mmHg</strong> e diastólica em até 10 mmHg, sem efeitos adversos significativos.",
    url: "https://pubmed.ncbi.nlm.nih.gov/17287847/"
  },
  {
    cat: "cardio",
    tag: "Revisão Volek",
    title: "Carbohydrate Restriction has a More Favorable Impact on the Metabolic Syndrome than a Low Fat Diet",
    authors: "Volek JS, Phinney SD, et al.",
    journal: "Lipids, 2009",
    finding: "Restrição de hidratos melhora as 5 componentes da síndrome metabólica de forma superior a dietas low-fat — incluindo redução notável de partículas LDL pequenas e densas (aterogénicas).",
    url: "https://pubmed.ncbi.nlm.nih.gov/19082851/"
  },
 
  // ===== CÉREBRO & MENTAL =====
  {
    cat: "brain",
    tag: "Cetose · Enxaqueca",
    title: "Migraine improvement during short lasting ketogenesis: a proof-of-concept study",
    authors: "Di Lorenzo C, et al.",
    journal: "European Journal of Neurology, 2015",
    finding: "Dieta cetogénica reduziu frequência de enxaqueca em <strong>80%</strong> dos pacientes em apenas 1 mês, com redução média de 3.7 dias com dor por mês. Efeito persistente após retorno a dieta normal.",
    url: "https://onlinelibrary.wiley.com/doi/10.1111/ene.12550"
  },
  {
    cat: "brain",
    tag: "Psiquiatria metabólica",
    title: "Ketogenic diet for the treatment of severe mental illness: a pilot study",
    authors: "Sethi S, et al. (Stanford)",
    journal: "Psychiatry Research, 2024",
    finding: "Em 21 pacientes com esquizofrenia ou bipolar: <strong>100%</strong> dos que aderiram à cetogénica mostraram melhoria psiquiátrica; 79% melhoria clinicamente significativa, com redução simultânea de marcadores metabólicos.",
    url: "https://www.sciencedirect.com/science/article/pii/S0165178124001513"
  },
  {
    cat: "brain",
    tag: "Cetose · Epilepsia",
    title: "A randomized trial of classical and medium-chain triglyceride ketogenic diets in the treatment of childhood epilepsy",
    authors: "Neal EG, et al.",
    journal: "Epilepsia, 2009",
    finding: "Estudo randomizado em 145 crianças com epilepsia refratária: dieta cetogénica reduziu convulsões em <strong>≥50%</strong> em 38% dos pacientes vs 6% no controlo. Eficácia comparável à de fármacos antiepilépticos.",
    url: "https://onlinelibrary.wiley.com/doi/10.1111/j.1528-1167.2008.01870.x"
  },
  {
    cat: "brain",
    tag: "Ómega-3 · Depressão",
    title: "Omega-3 fatty acids for the treatment of depressive disorders: a meta-analysis",
    authors: "Liao Y, et al.",
    journal: "Translational Psychiatry, 2019",
    finding: "Meta-análise de 26 estudos: ómega-3 com pelo menos 60% EPA mostrou efeito antidepressivo significativo, particularmente como terapia adjuvante a SSRIs.",
    url: "https://www.nature.com/articles/s41398-019-0515-5"
  },
 
  // ===== AUTOIMUNE & INFLAMAÇÃO =====
  {
    cat: "autoimmune",
    tag: "Hashimoto",
    title: "Selenium supplementation in the treatment of Hashimoto's thyroiditis: a systematic review and meta-analysis",
    authors: "Toulis KA, et al.",
    journal: "Thyroid, 2010",
    finding: "Suplementação de 200 mcg/dia de selenometionina reduziu significativamente anticorpos anti-TPO em pacientes com tiroidite de Hashimoto às 3 e 6 meses.",
    url: "https://pubmed.ncbi.nlm.nih.gov/20810577/"
  },
  {
    cat: "autoimmune",
    tag: "Vitamina D",
    title: "Vitamin D and autoimmune diseases: is vitamin D receptor (VDR) polymorphism the culprit?",
    authors: "Yamamoto EA, Jørgensen TN",
    journal: "Frontiers in Immunology, 2020",
    finding: "Revisão extensa demonstrando o papel central da vitamina D na regulação do sistema imune e como a deficiência está associada a maior risco e severidade de múltiplas autoimunes (LES, AR, EM, DT1).",
    url: "https://www.frontiersin.org/articles/10.3389/fimmu.2019.03141/full"
  },
  {
    cat: "autoimmune",
    tag: "AIP · Ensaio piloto",
    title: "Efficacy of the Autoimmune Protocol Diet for Inflammatory Bowel Disease",
    authors: "Konijeti GG, et al.",
    journal: "Inflammatory Bowel Diseases, 2017",
    finding: "Em 15 pacientes com Crohn ou colite ulcerosa: dieta paleo autoimune (AIP) atingiu remissão clínica em <strong>73%</strong> às 6 semanas, sustentada às 11 semanas, sem alterações de medicação.",
    url: "https://academic.oup.com/ibdjournal/article/23/11/2054/4791703"
  },
  {
    cat: "autoimmune",
    tag: "Curcumina · Artrite",
    title: "Efficacy and safety of curcumin and its combination with boswellic acid in osteoarthritis",
    authors: "Haroyan A, et al.",
    journal: "BMC Complementary Medicine and Therapies, 2018",
    finding: "Combinação curcumina + boswélia mostrou-se mais eficaz que curcumina isolada e <strong>comparável a AINEs</strong> na redução de dor e inflamação em osteoartrite, sem efeitos gastrointestinais adversos.",
    url: "https://bmccomplementmedtherapies.biomedcentral.com/articles/10.1186/s12906-017-2062-z"
  },
 
  // ===== HORMONAL =====
  {
    cat: "hormonal",
    tag: "SOP · Inositol",
    title: "Myo-inositol effects in women with PCOS: a meta-analysis of randomized controlled trials",
    authors: "Unfer V, et al.",
    journal: "Endocrine Connections, 2017",
    finding: "Meta-análise mostrou que myo-inositol melhora ovulação, reduz testosterona livre e melhora sensibilidade à insulina em mulheres com SOP, com perfil de segurança superior à metformina.",
    url: "https://ec.bioscientifica.com/view/journals/ec/6/8/EC-17-0243.xml"
  },
  {
    cat: "hormonal",
    tag: "Hipotiroidismo",
    title: "Effect of selenium supplementation on antithyroid peroxidase antibodies in subclinical hypothyroidism",
    authors: "Drutel A, Archambeaud F, Caron P",
    journal: "Clinical Endocrinology, 2013",
    finding: "Revisão dos efeitos benéficos do selénio em tiroidite autoimune — redução consistente de anticorpos anti-TPO e melhoria de marcadores de função tiroideia.",
    url: "https://onlinelibrary.wiley.com/doi/10.1111/cen.12066"
  },
  {
    cat: "hormonal",
    tag: "Vitamina D · Diabetes",
    title: "The role of vitamin D and calcium in type 2 diabetes",
    authors: "Pittas AG, Lau J, Hu FB, Dawson-Hughes B",
    journal: "Journal of Clinical Endocrinology &amp; Metabolism, 2007",
    finding: "Meta-análise estabelece relação inversa robusta entre níveis de 25(OH)D e prevalência de DT2 e síndrome metabólica. Suplementação melhora marcadores glicémicos.",
    url: "https://academic.oup.com/jcem/article/92/6/2017/2598434"
  },
 
  // ===== PESO & COMPOSIÇÃO =====
  {
    cat: "weight",
    tag: "Cetose · NAFLD",
    title: "Short-term weight loss and hepatic triglyceride reduction: evidence of a metabolic advantage with dietary carbohydrate restriction",
    authors: "Browning JD, et al.",
    journal: "American Journal of Clinical Nutrition, 2011",
    finding: "Em apenas <strong>2 semanas</strong> de dieta cetogénica, gordura hepática reduziu <strong>55%</strong> em pacientes com esteatose. Vantagem metabólica clara sobre dieta hipocalórica isocalórica.",
    url: "https://academic.oup.com/ajcn/article/93/5/1048/4597859"
  },
  {
    cat: "weight",
    tag: "Saciedade",
    title: "Effects of a high-protein ketogenic diet on hunger, appetite, and weight loss in obese men feeding ad libitum",
    authors: "Johnstone AM, et al.",
    journal: "American Journal of Clinical Nutrition, 2008",
    finding: "Dieta cetogénica ad libitum produziu redução espontânea da ingestão calórica e perda de peso significativa, com supressão da grelina e maior saciedade vs dieta moderada em hidratos.",
    url: "https://academic.oup.com/ajcn/article/87/1/44/4633297"
  },
  {
    cat: "weight",
    tag: "Termogénese",
    title: "Effects of a low carbohydrate diet on energy expenditure during weight loss maintenance",
    authors: "Ebbeling CB, et al.",
    journal: "BMJ, 2018",
    finding: "Estudo de 20 semanas mostrou que dieta low-carb aumentou o gasto energético em <strong>200-300 kcal/dia</strong> vs dieta high-carb com mesmas calorias — evidência da teoria insulina-carbohidrato.",
    url: "https://www.bmj.com/content/363/bmj.k4583"
  },
  {
    cat: "weight",
    tag: "Carnívora",
    title: "Behavioral characteristics and self-reported health status among 2029 adults consuming a 'carnivore diet'",
    authors: "Lennerz BS, et al. (Harvard)",
    journal: "Current Developments in Nutrition, 2021",
    finding: "Inquérito a 2029 adultos em dieta carnívora &gt;6 meses: <strong>93%</strong> reportaram melhoria ou resolução de problemas digestivos; 95% reportaram melhoria de energia, sono e composição corporal. Marcadores metabólicos médios excelentes.",
    url: "https://academic.oup.com/cdn/article/5/12/nzab133/6415894"
  },
 
  // ===== HISTÓRICOS =====
  {
    cat: "historical",
    tag: "Bellevue · 1928",
    title: "Prolonged Meat Diets with a Study of Kidney Function and Ketosis",
    authors: "McClellan WS, Du Bois EF",
    journal: "Journal of Biological Chemistry, 1930",
    finding: "Experimento clássico no Bellevue Hospital: Stefansson e Andersen viveram 1 ano sob supervisão médica consumindo apenas carne, gordura e órgãos. Sem deficiências nutricionais, melhoria de marcadores metabólicos.",
    url: "https://www.jbc.org/article/S0021-9258(18)76368-8/pdf"
  },
  {
    cat: "historical",
    tag: "Crítica histórica",
    title: "Re-evaluation of the traditional diet-heart hypothesis: analysis of recovered data from Minnesota Coronary Experiment",
    authors: "Ramsden CE, et al.",
    journal: "BMJ, 2016",
    finding: "Reanálise de dados perdidos do estudo Minnesota Coronary Experiment (1968): substituir gordura saturada por óleos vegetais ricos em ómega-6 reduziu colesterol mas <strong>aumentou mortalidade</strong> — desafiando 50 anos de orientação nutricional.",
    url: "https://www.bmj.com/content/353/bmj.i1246"
  },
  {
    cat: "historical",
    tag: "Antropologia · Dieta",
    title: "The Western diet and lifestyle and diseases of civilization",
    authors: "Cordain L, et al.",
    journal: "Research Reports in Clinical Cardiology, 2011",
    finding: "Revisão fundacional da hipótese evolutiva: as 'doenças da civilização' (obesidade, DT2, doença cardíaca, autoimunes) são raras em populações que mantêm dietas ancestrais e proliferam com a adoção da dieta ocidental.",
    url: "https://www.dovepress.com/the-western-diet-and-lifestyle-and-diseases-of-civilization-peer-reviewed-fulltext-article-RRCC"
  },
  {
    cat: "historical",
    tag: "Inuit · Cardiovascular",
    title: "The Composition of the Eskimo Food in North Western Greenland",
    authors: "Bang HO, Dyerberg J",
    journal: "American Journal of Clinical Nutrition, 1980",
    finding: "Estudo seminal sobre populações Inuit consumindo dieta com >70% gordura animal e ausência virtual de doença cardiovascular. Origem da investigação sobre ómega-3 e EPA.",
    url: "https://academic.oup.com/ajcn/article-abstract/33/12/2657/4691716"
  }
];
 
// Render studies
function renderStudies(category = "all") {
  const grid = document.getElementById("studies-grid");
  const filtered = category === "all" ? studies : studies.filter(s => s.cat === category);
  grid.innerHTML = filtered.map(s => `
    <div class="study-card">
      <span class="study-tag">${s.tag}</span>
      <h4>${s.title}</h4>
      <div class="study-meta"><strong>${s.authors}</strong> · ${s.journal}</div>
      <p class="study-finding">${s.finding}</p>
      <a class="study-link" href="${s.url}" target="_blank" rel="noopener noreferrer">Ler estudo original</a>
    </div>
  `).join("");
}
renderStudies();
 
// Filter pills
document.querySelectorAll(".filter-pill").forEach(pill => {
  pill.addEventListener("click", () => {
    document.querySelectorAll(".filter-pill").forEach(p => p.classList.remove("active"));
    pill.classList.add("active");
    renderStudies(pill.dataset.cat);
  });
});
 
// Smooth scroll for nav
document.querySelectorAll('a[href^="#"]').forEach(a => {
  a.addEventListener("click", e => {
    const target = document.querySelector(a.getAttribute("href"));
    if (target) {
      e.preventDefault();
      target.scrollIntoView({behavior:"smooth"});
    }
  });
});
 
/* ============================================
   ASSISTENTE CONVERSACIONAL (RAÍZES AI)
   ============================================ */
 
// ---- Base de conhecimento de alimentos ----
const foodDB = {
  // alimentos permitidos (carnívora/keto)
  allowed: {
    carne: { tier: "S", note: "Carne de ruminante (vaca, borrego) é a base. Privilegie cortes gordos com osso." },
    vaca: { tier: "S", note: "Excelente. Inclua cortes gordos (entrecôte, picanha) e órgãos (fígado 1x/semana)." },
    borrego: { tier: "S", note: "Excelente fonte de proteína e gordura saudável." },
    porco: { tier: "A", note: "Ok. Privilegiar pasto. Bacon de qualidade e costeletas com gordura são ótimos." },
    frango: { tier: "B", note: "Ok mas mais magro. Prefira coxas e pele em vez de peito. Idealmente do campo." },
    peru: { tier: "B", note: "Idem frango — magro. Combine sempre com gordura adicional." },
    peixe: { tier: "S", note: "Excelente. Privilegie peixe gordo (salmão selvagem, sardinhas, cavala, atum)." },
    salmao: { tier: "S", note: "Top — rico em ómega-3 e vitamina D. Selvagem &gt; cativeiro." },
    sardinhas: { tier: "S", note: "Provavelmente o alimento mais nutritivo do mundo. Coma em lata ou grelhadas." },
    bacalhau: { tier: "A", note: "Ótimo. Acompanhe com manteiga ou azeite — é peixe magro." },
    atum: { tier: "A", note: "Ok com moderação (mercúrio). Em azeite é melhor que em água." },
    ovos: { tier: "S", note: "Alimento perfeito. 3-6 por dia sem problema. Privilegie galinhas do campo." },
    ovo: { tier: "S", note: "Alimento perfeito. 3-6 por dia sem problema. Privilegie galinhas do campo." },
    manteiga: { tier: "S", note: "Sim — preferencialmente de pasto. Rica em vitamina K2 e butirato." },
    azeite: { tier: "S", note: "Excelente. Use cru ou em cozinhados a baixa temperatura. Extra virgem sempre." },
    banha: { tier: "A", note: "Tradicional, estável a altas temperaturas. Boa para fritar e estufar." },
    coco: { tier: "A", note: "Óleo de coco é excelente para cozinhar. Triglicéridos de cadeia média (MCT)." },
    abacate: { tier: "S", note: "Sim, ilimitado. Gordura monoinsaturada, potássio, fibra." },
    queijo: { tier: "A", note: "Ok se tolera lácteos. Privilegie curados (parmesão, gruyère). Evite processados." },
    iogurte: { tier: "A", note: "Apenas integral, natural, sem açúcar. Grego é excelente. Evite 'light' e com fruta." },
    nozes: { tier: "B", note: "Com moderação — densas em calorias. Macadâmia, nozes e amêndoas são as melhores." },
    brocolos: { tier: "A", note: "Sim. Excelente fonte de sulforafano. Salteados em manteiga." },
    espinafres: { tier: "A", note: "Sim. Cozinhados são melhor digeridos que crus." },
    couveflor: { tier: "A", note: "Versátil — pode substituir arroz e puré de batata." },
    courgette: { tier: "A", note: "Excelente. Pode fazer 'esparguete' de courgette." },
    pepino: { tier: "A", note: "Sim, baixíssimo em hidratos." },
    alface: { tier: "A", note: "Sim, base de saladas. Adicione sempre azeite generoso." },
    cogumelos: { tier: "A", note: "Sim. Saltear em manteiga ou azeite." },
    tomate: { tier: "B", note: "Ok com moderação. É fruto, tem alguma frutose." },
    cebola: { tier: "B", note: "Pequenas quantidades como tempero. Tem hidratos." },
    alho: { tier: "A", note: "Sim, como tempero. Anti-inflamatório natural." }
  },
  // alimentos a evitar
  avoid: {
    pao: { reason: "Trigo refinado, alto IG, aumenta inflamação intestinal e glicémia." },
    pão: { reason: "Trigo refinado, alto IG, aumenta inflamação intestinal e glicémia." },
    massa: { reason: "Hidrato refinado, sem valor nutricional, dispara insulina." },
    arroz: { reason: "Hidrato puro. Se mesmo necessário, prefira basmati ou jasmim em pouca quantidade." },
    batata: { reason: "Amido elevado. Substitua por couve-flor ou nabo." },
    açucar: { reason: "Veneno metabólico. Sem exceções." },
    açúcar: { reason: "Veneno metabólico. Sem exceções." },
    bolo: { reason: "Combinação tóxica de açúcar + farinha + óleos vegetais." },
    bolacha: { reason: "Ultra-processado. Açúcar, farinha, óleos refinados." },
    refrigerante: { reason: "Açúcar líquido. Pior ainda nos 'zero' (adoçantes desregulam apetite)." },
    sumo: { reason: "Mesmo natural — concentra frutose sem a fibra. Beba a fruta inteira." },
    cereais: { reason: "Pequeno-almoço dos cereais é um truque de marketing. Açúcar + grãos refinados." },
    margarina: { reason: "Óleos vegetais hidrogenados. Pior do que a manteiga em todos os parâmetros." },
    girassol: { reason: "Óleo de girassol é alto em ómega-6 inflamatório. Substitua por azeite ou manteiga." },
    soja: { reason: "Disruptor endócrino. Evitar especialmente em homens e crianças." },
    leguminosas: { reason: "Antinutrientes (lectinas, fitatos). Eliminar em protocolo terapêutico." }
  }
};
 
// ---- Mapeamento sintoma → patologia (chaves da pathologies já existente) ----
const symptomMap = {
  "fadiga": "fatigue", "cansaço": "fatigue", "cansada": "fatigue", "cansado": "fatigue", "sem energia": "fatigue",
  "esgotamento": "fatigue", "burnout": "fatigue", "exausto": "fatigue", "exausta": "fatigue",
  "dor de cabeça": "migraine", "enxaqueca": "migraine", "enxaquecas": "migraine", "cefaleia": "migraine",
  "dor articular": "inflammation", "dor nas articulações": "inflammation", "artrite": "inflammation",
  "artrose": "inflammation", "inflamação": "inflammation", "inchaço articular": "inflammation",
  "inchaço abdominal": "ibs", "barriga inchada": "ibs", "gases": "ibs", "intestino": "ibs",
  "obstipação": "ibs", "diarreia": "ibs", "sii": "ibs", "sibo": "ibs", "intestino irritável": "ibs",
  "azia": "reflux", "refluxo": "reflux", "ardor estômago": "reflux", "drge": "reflux",
  "ansiedade": "depression", "depressão": "depression", "depressao": "depression", "tristeza": "depression",
  "mau humor": "depression", "humor": "depression", "depressivo": "depression",
  "insónia": "insomnia", "insónias": "insomnia", "insónia": "insomnia", "dormir mal": "insomnia",
  "sono": "insomnia", "não consigo dormir": "insomnia",
  "diabetes": "diabetes", "glicose alta": "diabetes", "açúcar no sangue": "diabetes", "hba1c": "diabetes",
  "pré-diabetes": "diabetes", "resistência insulina": "diabetes",
  "tensão alta": "hypertension", "hipertensão": "hypertension", "pressão alta": "hypertension",
  "colesterol": "cholesterol", "triglicéridos": "cholesterol", "ldl alto": "cholesterol", "dislipidémia": "cholesterol",
  "ovário poliquístico": "pcos", "sop": "pcos", "ovários": "pcos", "ciclo irregular": "pcos",
  "tiroide": "hypothyroid", "tiróide": "hypothyroid", "hipotiroidismo": "hypothyroid", "hashimoto": "hypothyroid",
  "autoimune": "autoimmune", "lúpus": "autoimmune", "esclerose": "autoimmune", "artrite reumatoide": "autoimmune",
  "fígado gordo": "nafld", "esteatose": "nafld", "nafld": "nafld", "transaminases": "nafld",
  "osteoporose": "osteoporosis", "osteopenia": "osteoporosis", "ossos fracos": "osteoporosis",
  "síndrome metabólica": "metabolic", "obesidade abdominal": "metabolic"
};
 
// ---- Conversa ----
let chatHistory = [];
 
const greeting = `Olá! Sou a <strong>Raízes AI</strong>, a sua assistente. Posso ajudar com:
<ul>
  <li>🥩 Dúvidas sobre alimentos — <em>"posso comer X?"</em></li>
  <li>🩺 Sintomas e patologias — <em>"tenho enxaquecas"</em></li>
  <li>🧬 Recomendar suplementação — <em>"que tomar para ansiedade?"</em></li>
  <li>📊 Explicar princípios — <em>"o que é cetose?"</em></li>
</ul>
Em que lhe posso ser útil hoje?`;
 
const defaultSuggestions = [
  "Posso comer fruta?",
  "Tenho enxaquecas",
  "O que é cetose?",
  "Suplementos para ansiedade",
  "O que comer ao pequeno-almoço?",
  "Tenho diabetes tipo 2"
];
 
// ---- Lógica de interpretação ----
function normalize(text) {
  return text.toLowerCase()
    .replace(/[ãâá]/g, "a")
    .replace(/[éê]/g, "e")
    .replace(/[íî]/g, "i")
    .replace(/[óôõ]/g, "o")
    .replace(/[ú]/g, "u")
    .replace(/[ç]/g, "c")
    .replace(/[?!.,;:]/g, " ")
    .trim();
}
 
function findFood(text) {
  const t = normalize(text);
  const allFoods = { ...foodDB.allowed, ...foodDB.avoid };
  for (const food of Object.keys(allFoods)) {
    const f = normalize(food);
    if (t.includes(f)) return food;
  }
  return null;
}
 
function findSymptom(text) {
  const t = normalize(text);
  const matches = [];
  for (const [symptom, pathKey] of Object.entries(symptomMap)) {
    if (t.includes(normalize(symptom))) {
      if (!matches.some(m => m.path === pathKey)) {
        matches.push({ symptom, path: pathKey });
      }
    }
  }
  return matches;
}
 
function detectIntent(text) {
  const t = normalize(text);
 
  // Intent: comida específica
  if (/posso comer|posso beber|come(r)? |comida|alimento|come |beber|prato|refeicao|ementa|menu|pequeno-almoco|almoco|jantar|lanche|comer/.test(t)) {
    return "food";
  }
  // Intent: sintomas / patologias
  const symptoms = findSymptom(text);
  if (symptoms.length > 0) return "symptom";
 
  // Intent: suplementos
  if (/suplemento|tomar|toma |comprar|magnesio|omega|vitamina|colina|berberina|coq10|q10/.test(t)) {
    return "supplement";
  }
  // Intent: conceitos
  if (/o que e|porque |porque|como funciona|cetose|jejum|low.?carb|carnivora|keto|paleo|inflamacao|insulina/.test(t)) {
    return "concept";
  }
  // Intent: exemplo de menu
  if (/exemplo|sugest|menu|plano|dia|semana/.test(t)) {
    return "menu";
  }
 
  return "general";
}
 
// ---- Geradores de resposta ----
function answerFood(text) {
  const food = findFood(text);
  if (!food) {
    return `Não percebi qual o alimento. Pode dizer-me concretamente — por exemplo "posso comer banana?" ou "e queijo?". Posso também sugerir-lhe um plano completo se preferir — basta usar o <a href="#planeador">Planeador</a>.`;
  }
  if (foodDB.allowed[food]) {
    const info = foodDB.allowed[food];
    const tierLabel = { "S": "✅ Excelente — alimento ideal", "A": "✅ Sim, boa escolha", "B": "⚠️ Sim com moderação" }[info.tier];
    return `<strong>${food.charAt(0).toUpperCase() + food.slice(1)}</strong><br>${tierLabel}<br><br>${info.note}`;
  }
  if (foodDB.avoid[food]) {
    const info = foodDB.avoid[food];
    return `<strong>${food.charAt(0).toUpperCase() + food.slice(1)}</strong><br>❌ Não recomendado.<br><br>${info.reason}<br><br>Quer que sugira uma alternativa? Diga-me o que pretendia comer (ex: "queria algo doce" ou "queria acompanhar a carne").`;
  }
}
 
function answerSymptom(text) {
  const matches = findSymptom(text);
  if (matches.length === 0) return null;
 
  return matches.map(m => {
    const p = pathologies[m.path];
    if (!p) return "";
    const topSupps = p.supplements.slice(0, 3).map(([n, d, _]) =>
      `<div class="mini-table-row"><strong>${n}</strong><span>${d}</span></div>`
    ).join("");
    return `Detectei que mencionou <strong>"${m.symptom}"</strong> — pode estar relacionado com <strong>${p.name}</strong>.<br><br>
<em>Dieta sugerida:</em> ${p.diet}<br><br>
<em>Top 3 suplementos:</em>
<div class="mini-table">${topSupps}</div>
<br>Veja o detalhe completo (com base científica) na secção de <a href="#patologias">Suplementos</a>. Tem mais algum sintoma para me dizer?`;
  }).join("<br><br>━━━━━━━━━━<br><br>");
}
 
function answerSupplement(text) {
  const t = normalize(text);
  // Match supplement name to pathologies
  const supKeywords = {
    "magnesio": ["fatigue", "insomnia", "hypertension", "migraine"],
    "omega": ["cholesterol", "depression", "inflammation", "autoimmune"],
    "vitamina d": ["autoimmune", "depression", "osteoporosis", "hypothyroid"],
    "berberina": ["diabetes", "metabolic", "pcos"],
    "coq10": ["hypertension", "fatigue", "migraine"],
    "selenio": ["hypothyroid", "autoimmune"],
    "inositol": ["pcos", "metabolic", "nafld"],
    "curcumina": ["inflammation", "autoimmune"],
    "colina": ["nafld"],
    "k2": ["osteoporosis", "cholesterol"]
  };
 
  for (const [supp, paths] of Object.entries(supKeywords)) {
    if (t.includes(supp)) {
      const usefulFor = paths.map(p => pathologies[p]?.name).filter(Boolean);
      return `<strong>${supp.charAt(0).toUpperCase() + supp.slice(1)}</strong> é particularmente útil em:
<ul>${usefulFor.map(n => `<li>${n}</li>`).join("")}</ul>
Para dosagens exatas e mecanismo de ação, indique-me a sua patologia ou consulte directamente a secção de <a href="#patologias">Suplementos</a>.`;
    }
  }
 
  // Match "para X" pattern
  const symptoms = findSymptom(text);
  if (symptoms.length > 0) return answerSymptom(text);
 
  return `Para recomendar suplementos preciso de saber qual a sua condição. Diga-me, por exemplo: "que tomar para insónia?" ou "suplementos para diabetes". Em alternativa, selecione as suas patologias na secção de <a href="#patologias">Suplementos</a>.`;
}
 
function answerConcept(text) {
  const t = normalize(text);
  if (t.includes("cetose")) {
    return `<strong>Cetose nutricional</strong> é o estado metabólico em que o corpo, na ausência de hidratos de carbono suficientes, passa a usar <strong>corpos cetónicos</strong> (produzidos a partir de gordura) como combustível principal — em vez de glicose.<br><br>
É um estado <em>fisiológico</em> (diferente de cetoacidose, que é patológica). Tem benefícios documentados em epilepsia, diabetes, obesidade, doenças neurodegenerativas e várias autoimunes.<br><br>
Para entrar em cetose: hidratos &lt;30g/dia durante 2-3 semanas. Veja o <a href="#transicao">Protocolo de Transição</a>.`;
  }
  if (t.includes("jejum")) {
    return `<strong>Jejum intermitente</strong> é simplesmente comer dentro de uma janela de tempo (ex: 8h) e jejuar nas restantes (16h). Benefícios: melhora sensibilidade à insulina, ativa autofagia (limpeza celular), normaliza grelina (hormona da fome), simplifica a vida.<br><br>
Para começar: salte o pequeno-almoço, faça primeira refeição às 12h, última às 20h. Aumente gradualmente.`;
  }
  if (t.includes("carnivora") || t.includes("carnívora")) {
    return `A <strong>dieta carnívora</strong> é o protocolo de eliminação mais radical: apenas produtos animais (carne, peixe, ovos, vísceras, sal). Usada como ferramenta diagnóstica/terapêutica em casos resistentes — autoimunes severas, problemas digestivos crónicos, intolerâncias múltiplas.<br><br>
Não é uma dieta para sempre obrigatoriamente — muitos usam por 60-90 dias e depois reintroduzem alimentos para identificar gatilhos. Veja a Harvard study (Lennerz 2021) na secção <a href="#estudos">Estudos</a>.`;
  }
  if (t.includes("low") || t.includes("low-carb")) {
    return `<strong>Low-carb</strong> é a versão mais flexível: 50-100g de hidratos por dia, eliminando refinados (pão, açúcar, massas) mas mantendo vegetais, fruta de baixo IG e algumas raízes. Excelente ponto de partida e protocolo de manutenção a longo prazo.`;
  }
  if (t.includes("insulina") || t.includes("inflamacao")) {
    return `A <strong>resistência à insulina</strong> e a <strong>inflamação crónica</strong> são as duas raízes metabólicas da maior parte das doenças modernas. A insulina cronicamente elevada (causada por dieta rica em hidratos) bloqueia a queima de gordura, promove armazenamento e gera inflamação sistémica.<br><br>
A solução é simples: reduzir hidratos, eliminar açúcar e óleos refinados, comer comida real.`;
  }
  return `Boa pergunta — pode reformular para que eu perceba melhor? Posso explicar conceitos como cetose, jejum intermitente, dieta carnívora, low-carb, ou resistência à insulina.`;
}
 
function answerMenu(text) {
  const t = normalize(text);
  if (t.includes("pequeno-almoco") || t.includes("pequeno almoco")) {
    return `Sugestões de <strong>pequeno-almoço</strong> low-carb/keto:
<ul>
  <li>2-3 ovos mexidos em manteiga + bacon + abacate</li>
  <li>Omelete com queijo curado e cogumelos</li>
  <li>Iogurte grego integral + frutos vermelhos + nozes</li>
  <li>Café bulletproof (café + manteiga + óleo MCT) — ideal para jejum prolongado</li>
  <li>Salmão fumado + ovo cozido + abacate</li>
</ul>
Ou simplesmente <em>saltar o pequeno-almoço</em> — o jejum até ao almoço é uma das ferramentas mais poderosas.`;
  }
  if (t.includes("almoco")) {
    return `Sugestões de <strong>almoço</strong>:
<ul>
  <li>Bife grelhado + salada de espinafres com azeite e abacate</li>
  <li>Salmão em manteiga + brócolos salteados</li>
  <li>Frango assado com pele + couve-flor</li>
  <li>Hambúrguer caseiro (sem pão) + salada + bacon</li>
  <li>Atum em azeite + ovo cozido + alface + tomate</li>
</ul>`;
  }
  if (t.includes("jantar")) {
    return `Sugestões de <strong>jantar</strong>:
<ul>
  <li>Sardinhas grelhadas + salada de tomate</li>
  <li>Costeletas de borrego + courgette grelhada</li>
  <li>Bacalhau fresco + grelos salteados em alho</li>
  <li>Picanha + cogumelos em manteiga</li>
  <li>Sopa de legumes + ovos cozidos</li>
</ul>`;
  }
  return `Quer um plano semanal completo? Use o <a href="#planeador">Planeador</a> — em 5 perguntas devolve menu de 7 dias adaptado ao seu objetivo.`;
}
 
function answerGeneral(text) {
  const t = normalize(text);
  if (/oi|ola|bom dia|boa tarde|boa noite|hello/.test(t)) {
    return "Olá! Como posso ajudar — dúvidas sobre alimentos, sintomas, suplementos?";
  }
  if (/obrigad|valeu|ok|certo/.test(t)) {
    return "De nada! Estou aqui se precisar de mais alguma coisa. 🌱";
  }
  return `Não tenho a certeza do que pergunta. Pode reformular? Algumas coisas em que posso ajudar:
<ul>
  <li>"Posso comer [alimento]?"</li>
  <li>"Tenho [sintoma/patologia]"</li>
  <li>"Suplementos para [condição]"</li>
  <li>"O que é [conceito]?"</li>
  <li>"Sugestões de [refeição]"</li>
</ul>`;
}
 
function generateResponse(text) {
  const intent = detectIntent(text);
  switch (intent) {
    case "food": return answerFood(text);
    case "symptom": return answerSymptom(text) || answerGeneral(text);
    case "supplement": return answerSupplement(text);
    case "concept": return answerConcept(text);
    case "menu": return answerMenu(text);
    default: return answerGeneral(text);
  }
}
 
// ---- UI helpers ----
function addMessage(content, role) {
  const messages = document.getElementById("chat-messages");
  const msg = document.createElement("div");
  msg.className = "msg msg-" + role;
  msg.innerHTML = `<div class="msg-bubble">${content}</div>`;
  messages.appendChild(msg);
  messages.scrollTop = messages.scrollHeight;
  chatHistory.push({ role, content });
}
 
function showTyping() {
  const messages = document.getElementById("chat-messages");
  const typing = document.createElement("div");
  typing.className = "typing";
  typing.id = "typing-indicator";
  typing.innerHTML = "<span></span><span></span><span></span>";
  messages.appendChild(typing);
  messages.scrollTop = messages.scrollHeight;
}
 
function hideTyping() {
  document.getElementById("typing-indicator")?.remove();
}
 
function renderSuggestions(arr) {
  const container = document.getElementById("chat-suggestions");
  container.innerHTML = arr.map(s => `<button class="suggestion-chip">${s}</button>`).join("");
  container.querySelectorAll(".suggestion-chip").forEach(chip => {
    chip.addEventListener("click", () => {
      sendMessage(chip.textContent);
    });
  });
}
 
function generateContextSuggestions(lastResponse) {
  const r = lastResponse.toLowerCase();
  if (r.includes("patologia") || r.includes("dieta sugerida")) {
    return ["Que comer ao pequeno-almoço?", "Tenho mais sintomas", "Como começar?"];
  }
  if (r.includes("alimento ideal") || r.includes("não recomendado")) {
    return ["E sobremesa?", "Que beber?", "Mais sugestões"];
  }
  if (r.includes("cetose")) {
    return ["Como entrar em cetose?", "Quanto tempo demora?", "Sintomas da keto-flu"];
  }
  return defaultSuggestions.slice(0, 4);
}
 
function sendMessage(text) {
  if (!text.trim()) return;
  addMessage(escapeHtml(text), "user");
  document.getElementById("chat-input").value = "";
  showTyping();
  const delay = 600 + Math.random() * 700;
  setTimeout(() => {
    hideTyping();
    const response = generateResponse(text);
    addMessage(response, "bot");
    renderSuggestions(generateContextSuggestions(response));
  }, delay);
}
 
function escapeHtml(s) {
  return s.replace(/[&<>"']/g, c => ({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]));
}
 
// ---- Init chat ----
document.getElementById("chat-fab").addEventListener("click", () => {
  document.getElementById("chat-panel").classList.add("open");
  document.getElementById("chat-fab").classList.add("hidden");
  document.getElementById("chat-fab-label").style.display = "none";
  if (chatHistory.length === 0) {
    addMessage(greeting, "bot");
    renderSuggestions(defaultSuggestions);
  }
});
document.getElementById("chat-close").addEventListener("click", () => {
  document.getElementById("chat-panel").classList.remove("open");
  document.getElementById("chat-fab").classList.remove("hidden");
});
document.getElementById("chat-send").addEventListener("click", () => {
  sendMessage(document.getElementById("chat-input").value);
});
document.getElementById("chat-input").addEventListener("keydown", e => {
  if (e.key === "Enter" && !e.shiftKey) {
    e.preventDefault();
    sendMessage(e.target.value);
  }
});
// Auto-resize textarea
document.getElementById("chat-input").addEventListener("input", e => {
  e.target.style.height = "auto";
  e.target.style.height = Math.min(e.target.scrollHeight, 100) + "px";
});
</script>
 
</body>
</html>
 
