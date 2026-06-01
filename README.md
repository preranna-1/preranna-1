<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>✨ Prerana Thapa Magar · pastel dev & data whisperer ✨</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: linear-gradient(145deg, #fff9f5 0%, #ffe8f0 100%);
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', 'Helvetica Neue', sans-serif;
      padding: 2rem 1.5rem;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    /* main pastel card */
    .profile-card {
      max-width: 1100px;
      width: 100%;
      margin: 0 auto;
      background: rgba(255, 251, 245, 0.9);
      backdrop-filter: blur(2px);
      border-radius: 2.5rem;
      padding: 2.2rem;
      box-shadow: 0 20px 35px -12px rgba(0, 0, 0, 0.08), 0 1px 2px rgba(0,0,0,0.02);
      border: 1px solid #ffe0d4;
      transition: all 0.2s ease;
    }

    /* header area */
    .header {
      text-align: center;
      margin-bottom: 2rem;
    }

    .name {
      font-size: 2.8rem;
      font-weight: 700;
      background: linear-gradient(135deg, #F6A7C1, #FBC8B5);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      letter-spacing: -0.3px;
      display: inline-flex;
      align-items: center;
      gap: 12px;
      flex-wrap: wrap;
      justify-content: center;
    }

    .badge-row {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 12px;
      margin: 1rem 0 0.5rem;
    }

    .badge {
      background: #ffe3d6;
      padding: 6px 14px;
      border-radius: 60px;
      font-size: 0.8rem;
      font-weight: 500;
      color: #b15e3e;
      box-shadow: 0 1px 3px rgba(0,0,0,0.02);
    }

    .quote {
      font-style: italic;
      color: #e27c5a;
      background: #fff0e8;
      display: inline-block;
      padding: 0.4rem 1.2rem;
      border-radius: 80px;
      font-size: 0.9rem;
      margin-top: 12px;
    }

    /* two column layout */
    .two-columns {
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
      margin-top: 1rem;
    }

    .left {
      flex: 1.5;
      min-width: 220px;
    }

    .right {
      flex: 1;
      min-width: 240px;
    }

    /* sections */
    .section {
      background: #fffaf5;
      border-radius: 1.8rem;
      padding: 1.2rem 1.5rem;
      margin-bottom: 1.5rem;
      box-shadow: 0 4px 12px rgba(0,0,0,0.02);
      border: 1px solid #ffe1d0;
    }

    .section h3 {
      font-size: 1.3rem;
      font-weight: 600;
      margin-bottom: 1rem;
      color: #d sixteen;
      display: flex;
      align-items: center;
      gap: 8px;
      border-left: 4px solid #ffb48a;
      padding-left: 12px;
    }

    .code-block {
      background: #fef3ed;
      border-radius: 1.2rem;
      padding: 1rem;
      font-family: 'JetBrains Mono', 'Fira Code', monospace;
      font-size: 0.8rem;
      color: #7a4a38;
      border: 1px solid #ffd9c4;
      overflow-x: auto;
      white-space: pre-wrap;
      word-break: break-word;
    }

    .tech-grid {
      display: flex;
      flex-direction: column;
      gap: 0.8rem;
    }

    .tech-line {
      font-family: monospace;
      font-size: 0.85rem;
      padding: 6px 0;
      border-bottom: 1px dashed #ffd5bd;
    }

    .tech-label {
      font-weight: 700;
      color: #cf7652;
      display: inline-block;
      width: 105px;
    }

    .skill-tag {
      background: white;
      padding: 4px 12px;
      border-radius: 30px;
      font-size: 0.75rem;
      font-weight: 500;
      margin-right: 6px;
      margin-bottom: 6px;
      display: inline-block;
      color: #865d48;
      box-shadow: 0 1px 2px rgba(0,0,0,0.02);
    }

    .open-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 8px;
    }

    .open-tag {
      background: #ffe3d4;
      padding: 5px 14px;
      border-radius: 40px;
      font-size: 0.75rem;
      font-weight: 600;
      color: #c26340;
    }

    .findme-icons {
      display: flex;
      gap: 15px;
      flex-wrap: wrap;
      margin-top: 12px;
    }

    .findme-icons a {
      text-decoration: none;
      background: #ffefe5;
      padding: 6px 16px;
      border-radius: 40px;
      font-size: 0.8rem;
      font-weight: 500;
      color: #b55734;
      transition: 0.1s ease;
      display: inline-flex;
      align-items: center;
      gap: 6px;
    }

    .findme-icons a:hover {
      background: #ffd9c6;
      transform: scale(0.97);
    }

    hr {
      margin: 20px 0;
      border: 0;
      height: 2px;
      background: linear-gradient(to right, #ffcdb3, transparent);
    }

    .footer-note {
      text-align: center;
      font-size: 0.7rem;
      color: #d99474;
      margin-top: 1rem;
      letter-spacing: 0.3px;
    }

    @media (max-width: 700px) {
      .profile-card {
        padding: 1.5rem;
      }
      .name {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>
<div class="profile-card">
  
  <!-- header with cute pastel vibe -->
  <div class="header">
    <div class="name">
      🌸 Prerana Thapa Magar 🌼
    </div>
    <div class="badge-row">
      <span class="badge">📍 Gorkha, Nepal</span>
      <span class="badge">🎓 CS final year student</span>
      <span class="badge">🐞 bugmaker & breaker</span>
    </div>
    <div class="quote">
      ✨ “skilled in both debugging AND bugmaking — it's a superpower” ✨
    </div>
  </div>

  <div class="two-columns">
    <!-- LEFT COLUMN: bio, fun stuff, open to -->
    <div class="left">
      <div class="section">
        <h3>🧸 about.me()</h3>
        <div class="code-block">
          const me = {<br>
          &nbsp;&nbsp;name: "Prerana Thapa Magar",<br>
          &nbsp;&nbsp;location: "🌍 Gorkha, Nepal",<br>
          &nbsp;&nbsp;role: "CS final year student",<br>
          &nbsp;&nbsp;currently: "Building something awesome...",<br>
          &nbsp;&nbsp;funFact: "debugging & bugmaking duo",<br>
          &nbsp;&nbsp;openTo: ["collaborations", "open source", "freelance"]<br>
          };
        </div>
      </div>

      <div class="section">
        <h3>✨ what i actually do (cooler version)</h3>
        <p style="color:#7a4a38; line-height:1.5; font-size:0.9rem;">
          I design frontend stories, train image classifiers that spot patterns others miss, and build ML models that actually make sense of data. 
          I've designed backend models from scratch, and I genuinely enjoy making data look beautiful while telling a story. 
          Basically: <strong>data + design + code</strong>, all in one messy, wonderful sandwich.
        </p>
      </div>

      <div class="section">
        <h3>🤝 open to</h3>
        <div class="open-tags">
          <span class="open-tag">🤍 collaborations</span>
          <span class="open-tag">🌱 open source</span>
          <span class="open-tag">💸 freelance / design quests</span>
          <span class="open-tag">🐞 intentional bugmaking</span>
        </div>
      </div>
    </div>

    <!-- RIGHT COLUMN: tech stack & find me -->
    <div class="right">
      <div class="section">
        <h3>🧰 tech I speak</h3>
        <div class="tech-grid">
          <div class="tech-line">
            <span class="tech-label">languages :</span> 
            <span class="skill-tag">C</span>
            <span class="skill-tag">JAVA</span>
            <span class="skill-tag">PYTHON</span>
            <span class="skill-tag">JAVASCRIPT</span>
          </div>
          <div class="tech-line">
            <span class="tech-label">frontend :</span> 
            <span class="skill-tag">HTML</span>
            <span class="skill-tag">CSS</span>
            <span class="skill-tag">– making pixels feel pretty</span>
          </div>
          <div class="tech-line">
            <span class="tech-label">backend :</span> 
            <span class="skill-tag">Node.js</span>
            <span class="skill-tag">MySQL</span>
            <span class="skill-tag">XAMPP</span>
            <span class="skill-tag">– where data comes to life</span>
          </div>
          <div class="tech-line">
            <span class="tech-label">also into :</span> 
            <span class="skill-tag">frontend designs</span>
            <span class="skill-tag">ML models</span>
            <span class="skill-tag">image classification</span>
            <span class="skill-tag">data wrangling</span>
          </div>
        </div>
        <!-- additional code-block format as requested -->
        <div style="margin-top: 1rem;">
          <div class="code-block" style="font-size:0.75rem;">
            ╭─────────────────────────────────────────────────╮<br>
            │ 🧰 tech I speak                                 │<br>
            ├─────────────────────────────────────────────────┤<br>
            │ languages      : C • JAVA • PYTHON • JAVASCRIPT │<br>
            │ frontend       : HTML • CSS – pixels → pretty   │<br>
            │ backend        : Node.js • MySQL • XAMPP        │<br>
            │ also into      : frontend designs, ML models,   │<br>
            │                  image classification, data wrangling │<br>
            ╰─────────────────────────────────────────────────╯
          </div>
        </div>
      </div>

      <div class="section">
        <h3>🌊 find me · connect</h3>
        <div class="findme-icons">
          <a href="#">🐙 GitHub</a>
          <a href="#">🔗 LinkedIn</a>
          <a href="#">📧 Email</a>
          <a href="#">✨ Portfolio</a>
        </div>
        <p style="font-size:0.7rem; margin-top: 12px; color:#cb825f;">(replace with your actual links — these are placeholders 💌)</p>
      </div>

      <!-- simple github stats vibe (placeholder but looks cute) -->
      <div class="section">
        <h3>📊 code garden snapshot</h3>
        <div style="background:#fef0e8; border-radius: 1rem; padding: 0.8rem; text-align: center;">
          <div style="display: flex; justify-content: space-between; gap: 8px; font-size: 0.7rem; flex-wrap:wrap;">
            <span>⭐ 42 contributions this week</span>
            <span>🍀 11 repos brewing</span>
            <span>🐞 3 bugs intentionally left</span>
          </div>
          <div style="margin-top: 12px; background:#ffdfce; height: 6px; border-radius: 10px; width: 100%;">
            <div style="width: 73%; background:#ff9f7c; height: 6px; border-radius: 10px;"></div>
          </div>
          <div style="font-size:0.6rem; margin-top: 8px;">✨ pastel-powered ✨</div>
        </div>
      </div>
    </div>
  </div>

  <hr />
  <div class="footer-note">
    🌼 built with chai, curly braces & pastel dreams — currently building something awesome... 🌸
  </div>
</div>
</body>
</html>
