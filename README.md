<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
  <title>✨ Prerana Thapa Magar | magical dev & data alchemist ✨</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: linear-gradient(145deg, #f9f3e8 0%, #ffe6dc 100%);
      font-family: 'Inter', sans-serif;
      padding: 2rem 1.5rem;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="%23ff8a5c"><circle cx="12" cy="12" r="10" fill="%23ffb48a" stroke="%23e86a3f" stroke-width="1.5"/><circle cx="9" cy="9" r="1.5" fill="white"/><circle cx="15" cy="9" r="1.5" fill="white"/><path d="M8 15 Q12 18 16 15" stroke="%23a53f2b" stroke-width="1.5" fill="none"/></svg>') 12 12, auto;
    }

    /* main card container */
    .magic-card {
      max-width: 1300px;
      width: 100%;
      margin: 0 auto;
      background: rgba(255, 250, 240, 0.75);
      backdrop-filter: blur(6px);
      border-radius: 3rem;
      padding: 2rem 2rem 2rem 2rem;
      box-shadow: 0 25px 45px -12px rgba(0, 0, 0, 0.2), 0 0 0 1px rgba(255, 245, 225, 0.6);
      transition: all 0.2s ease;
    }

    /* layout grid */
    .profile-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
      justify-content: space-between;
    }

    .info-panel {
      flex: 2;
      min-width: 260px;
    }

    .play-panel {
      flex: 1.5;
      min-width: 320px;
      display: flex;
      flex-direction: column;
      gap: 1.8rem;
    }

    /* headings and text */
    .greeting {
      font-size: 1rem;
      letter-spacing: -0.2px;
      color: #e87a5a;
      font-weight: 500;
      text-transform: uppercase;
      margin-bottom: 0.5rem;
    }

    h1 {
      font-size: 2.8rem;
      font-weight: 700;
      background: linear-gradient(135deg, #D96C4E, #B84A2E);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      letter-spacing: -0.02em;
      margin-bottom: 0.5rem;
    }

    .location-role {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      margin-bottom: 1.5rem;
      color: #836953;
      font-weight: 500;
    }

    .chip {
      background: #fff0e6;
      padding: 0.3rem 1rem;
      border-radius: 60px;
      font-size: 0.85rem;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      backdrop-filter: blur(2px);
      box-shadow: 0 1px 2px rgba(0,0,0,0.02);
    }

    .fun-fact {
      background: #fde7dd;
      border-left: 5px solid #ff9f7c;
      padding: 1rem 1.2rem;
      border-radius: 24px;
      margin: 1.2rem 0;
      font-size: 0.9rem;
      font-weight: 500;
      color: #a45a3e;
    }

    .skill-section {
      margin: 1.5rem 0;
    }

    .skill-badge {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin: 10px 0 15px;
    }

    .badge {
      background: white;
      padding: 6px 14px;
      border-radius: 100px;
      font-size: 0.75rem;
      font-weight: 600;
      box-shadow: 0 2px 5px rgba(0,0,0,0.02);
      color: #5d3a2a;
      transition: 0.1s ease;
    }

    .badge-lg {
      background: #ffddd1;
      font-weight: 600;
    }

    .skill-desc {
      background: rgba(255, 235, 220, 0.6);
      padding: 1rem 1.2rem;
      border-radius: 28px;
      font-weight: 500;
      line-height: 1.4;
      font-size: 0.9rem;
      color: #794f38;
      margin-top: 1rem;
    }

    .open-to {
      margin-top: 1.8rem;
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem;
    }

    .open-tag {
      background: #f5e4d9;
      border-radius: 40px;
      padding: 0.3rem 1rem;
      font-size: 0.8rem;
      font-weight: 500;
      color: #b46444;
    }

    /* rotating avatar container */
    .avatar-cosmic {
      position: relative;
      width: 220px;
      height: 220px;
      margin: 0 auto;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .core-avatar {
      width: 130px;
      height: 130px;
      background: #ffdbbf;
      border-radius: 50%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      box-shadow: 0 15px 25px rgba(0,0,0,0.1), 0 0 0 6px #fff6ed;
      transition: all 0.2s;
      z-index: 3;
      backdrop-filter: blur(2px);
    }

    .avatar-emoji {
      font-size: 4rem;
      margin-bottom: 4px;
    }

    .avatar-name-mini {
      font-size: 0.7rem;
      font-weight: 600;
      background: #ffc8ae;
      padding: 2px 12px;
      border-radius: 30px;
      color: #593221;
    }

    .orbit-item {
      position: absolute;
      width: 40px;
      height: 40px;
      background: rgba(255, 249, 240, 0.9);
      backdrop-filter: blur(4px);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.4rem;
      box-shadow: 0 5px 12px rgba(0,0,0,0.05);
      transition: 0.05s linear;
      z-index: 5;
      pointer-events: none;
      border: 1px solid #ffe1cf;
    }

    /* pinball game area */
    .game-container {
      background: #f9ebdf;
      border-radius: 2rem;
      padding: 1rem;
      box-shadow: inset 0 0 0 1px #fffbf5, 0 12px 24px -10px rgba(0,0,0,0.1);
    }

    .game-header {
      display: flex;
      justify-content: space-between;
      font-weight: 700;
      padding: 0 0.5rem 0.7rem;
      color: #b35938;
    }

    canvas {
      display: block;
      margin: 0 auto;
      border-radius: 24px;
      background: #fef3ea;
      box-shadow: 0 2px 8px rgba(0,0,0,0.05);
      cursor: pointer;
      width: 100%;
      height: auto;
    }

    .game-footer {
      font-size: 0.7rem;
      text-align: center;
      margin-top: 0.7rem;
      color: #b67658;
      font-weight: 500;
    }

    hr {
      margin: 20px 0;
      border: 0;
      height: 2px;
      background: linear-gradient(to right, #ffd2bc, transparent);
    }

    @media (max-width: 820px) {
      .magic-card {
        padding: 1.5rem;
      }
      h1 {
        font-size: 2rem;
      }
      .avatar-cosmic {
        width: 180px;
        height: 180px;
      }
      .core-avatar {
        width: 100px;
        height: 100px;
      }
      .avatar-emoji {
        font-size: 3rem;
      }
      .orbit-item {
        width: 32px;
        height: 32px;
        font-size: 1.1rem;
      }
    }
  </style>
</head>
<body>

<div class="magic-card">
  <div class="profile-grid">
    <!-- LEFT: all bio + skills -->
    <div class="info-panel">
      <div class="greeting">✨ ༺ 𝐬𝐲𝐧𝐭𝐚𝐱 𝐬𝐨𝐫𝐜𝐞𝐫𝐞𝐬𝐬 ༻ ✨</div>
      <h1>Prerana Thapa Magar</h1>
      <div class="location-role">
        <span class="chip">📍 Gorkha, Nepal 🌄</span>
        <span class="chip">🎓 CS final year · bug maker & breaker</span>
      </div>
      <div class="fun-fact">
        ⚡ fun fact: “I am skilled in both debugging AND bugmaking — yes, it's a superpower”
      </div>
      <div class="skill-section">
        <div style="font-weight: 600; margin-bottom: 5px;">🗣️ languages spoken to machines</div>
        <div class="skill-badge">
          <span class="badge">C</span><span class="badge">JAVA</span><span class="badge">PYTHON</span><span class="badge">JAVASCRIPT</span>
        </div>
        <div style="font-weight: 600; margin-bottom: 5px; margin-top: 12px;">🎨 front-end spells</div>
        <div class="skill-badge">
          <span class="badge">HTML5</span><span class="badge">CSS3</span>
        </div>
        <div style="font-weight: 600; margin-bottom: 5px;">⚙️ back-end alchemy</div>
        <div class="skill-badge">
          <span class="badge">Node.js</span><span class="badge">MySQL</span><span class="badge">XAMPP</span>
        </div>
      </div>

      <!-- cool skill description (data + design + models) -->
      <div class="skill-desc">
        🌊 **data daydreamer & digital architect** <br>
        ➜ sculpting frontend stories • training image classifiers that see magic • weaving ML models that whisper insights <br>
        ➜ backend model designer • data alchemist turning raw bits into stories. <br>
        <span style="font-size:0.8rem; display:inline-block; margin-top:6px;">✨ currently: building something cosmic + cute</span>
      </div>

      <div class="open-to">
        <span class="open-tag">🤝 collaborations</span>
        <span class="open-tag">🌱 open source</span>
        <span class="open-tag">💸 freelance / design quests</span>
        <span class="open-tag">🐞 bugmaking (on purpose)</span>
      </div>
      <hr />
      <div style="font-size: 0.8rem; color:#b46444; text-align: right; font-weight: 500;">“designing the future one pixel & probability at a time”</div>
    </div>

    <!-- RIGHT PANEL: moving head + pinball joy -->
    <div class="play-panel">
      <!-- orbiting magical head zone -->
      <div class="avatar-cosmic" id="cosmicZone">
        <div class="core-avatar">
          <div class="avatar-emoji">🧸💻</div>
          <div class="avatar-name-mini">prerana.exe</div>
          <div style="font-size: 0.6rem; margin-top: 5px;">✨ 🌙 ✨</div>
        </div>
        <!-- these children will be moved dynamically (orbiting icons) -->
        <div class="orbit-item" id="orb0">🎨</div>
        <div class="orbit-item" id="orb1">🤖</div>
        <div class="orbit-item" id="orb2">📊</div>
        <div class="orbit-item" id="orb3">⚡</div>
        <div class="orbit-item" id="orb4">🧠</div>
        <div class="orbit-item" id="orb5">🐞</div>
        <div class="orbit-item" id="orb6">✨</div>
      </div>

      <!-- pinball mini game: cute and bouncy -->
      <div class="game-container">
        <div class="game-header">
          <span>🌀 PIN·BALL DREAMS 🎈</span>
          <span>💥 SCORE: <span id="scoreDisplay">0</span> &nbsp; ❤️ <span id="livesDisplay">3</span></span>
        </div>
        <canvas id="pinballCanvas" width="400" height="400" style="width:100%; height:auto; max-width:400px; aspect-ratio:1/1"></canvas>
        <div class="game-footer">
          🖱️ move mouse left/right → paddle floats | bumpers give +10 | don't let the ball fall!
        </div>
      </div>
    </div>
  </div>
</div>

<script>
  // ---------- ROTATING ORBIT MAGIC (cute items around head) ----------
  const orbitCenter = () => {
    const container = document.getElementById('cosmicZone');
    if(!container) return {x:0, y:0};
    const rect = container.getBoundingClientRect();
    // relative to container center
    return { cx: rect.width/2, cy: rect.height/2 };
  };
  
  const orbitItems = [
    document.getElementById('orb0'),
    document.getElementById('orb1'),
    document.getElementById('orb2'),
    document.getElementById('orb3'),
    document.getElementById('orb4'),
    document.getElementById('orb5'),
    document.getElementById('orb6')
  ];
  
  // orbit configuration: radius, speed, start angle offsets
  const orbits = [
    { radius: 85, speed: 0.008, angle: 0 },
    { radius: 100, speed: 0.005, angle: 1.2 },
    { radius: 75, speed: 0.01, angle: 2.5 },
    { radius: 95, speed: 0.007, angle: 3.0 },
    { radius: 110, speed: 0.004, angle: 4.1 },
    { radius: 80, speed: 0.009, angle: 5.3 },
    { radius: 105, speed: 0.006, angle: 0.9 }
  ];
  
  let angles = orbits.map(o => o.angle);
  let lastTimestamp = 0;
  
  function updateOrbitPositions() {
    const container = document.getElementById('cosmicZone');
    if(!container) return;
    const rect = container.getBoundingClientRect();
    const containerWidth = rect.width;
    const containerHeight = rect.height;
    const centerX = containerWidth / 2;
    const centerY = containerHeight / 2;
    if(containerWidth === 0) return;
    
    for(let i = 0; i < orbitItems.length; i++) {
      const item = orbitItems[i];
      if(!item) continue;
      const orbit = orbits[i];
      angles[i] += orbit.speed;
      const x = centerX + Math.cos(angles[i]) * orbit.radius;
      const y = centerY + Math.sin(angles[i]) * orbit.radius * 0.9; // slight vertical squash for cuteness
      item.style.left = (x - 20) + 'px';  // half width approx 20px
      item.style.top = (y - 20) + 'px';
    }
    requestAnimationFrame(() => updateOrbitPositions());
  }
  
  // start orbiting stars
  updateOrbitPositions();
  
  // ---------- PINBALL GAME (lightweight, cute bumper mayhem) ----------
  const canvas = document.getElementById('pinballCanvas');
  const ctx = canvas.getContext('2d');
  
  // dimensions
  let width = 400, height = 400;
  canvas.width = width;
  canvas.height = height;
  
  // ball properties
  let ball = {
    x: width/2,
    y: height - 70,
    r: 6,
    vx: 2.3,
    vy: -3.2
  };
  
  let paddle = {
    w: 70,
    h: 12,
    x: width/2 - 35,
    y: height - 20,
  };
  
  // bumpers: cute circular bumpers
  const bumpers = [
    { x: 80, y: 80, r: 12 },
    { x: 200, y: 60, r: 12 },
    { x: 320, y: 90, r: 12 },
    { x: 130, y: 150, r: 12 },
    { x: 270, y: 160, r: 12 },
    { x: 200, y: 210, r: 12 },
    { x: 340, y: 200, r: 10 },
    { x: 60, y: 210, r: 10 }
  ];
  
  let score = 0;
  let lives = 3;
  let gameActive = true;
  
  const scoreSpan = document.getElementById('scoreDisplay');
  const livesSpan = document.getElementById('livesDisplay');
  
  function updateUI() {
    scoreSpan.innerText = score;
    livesSpan.innerText = lives;
  }
  
  function resetBall() {
    ball.x = width/2;
    ball.y = height - 60;
    ball.vx = (Math.random() - 0.5) * 3.8;
    if(Math.abs(ball.vx) < 1) ball.vx = ball.vx > 0 ? 1.8 : -1.8;
    ball.vy = -3.2;
    // avoid infinite loop if stuck boundaries
    if(ball.y + ball.r >= height) ball.y = height - 50;
  }
  
  function loseLife() {
    lives--;
    updateUI();
    if(lives <= 0) {
      // game over reset score and lives
      score = 0;
      lives = 3;
      updateUI();
      resetBall();
    } else {
      resetBall();
    }
  }
  
  // collision helpers
  function handleWallCollision() {
    // left/right
    if(ball.x - ball.r <= 0) {
      ball.x = ball.r;
      ball.vx = -ball.vx;
    }
    if(ball.x + ball.r >= width) {
      ball.x = width - ball.r;
      ball.vx = -ball.vx;
    }
    // top
    if(ball.y - ball.r <= 0) {
      ball.y = ball.r;
      ball.vy = -ball.vy;
    }
    // bottom (lost life)
    if(ball.y + ball.r >= height + 8) {
      loseLife();
      return true;
    }
    return false;
  }
  
  function handlePaddleCollision() {
    if(ball.y + ball.r >= paddle.y && ball.y - ball.r <= paddle.y + paddle.h &&
       ball.x + ball.r >= paddle.x && ball.x - ball.r <= paddle.x + paddle.w) {
      // reflect based on hit position
      let hitPos = (ball.x - paddle.x) / paddle.w;
      let angle = (hitPos - 0.5) * 1.6; // -0.8..0.8 rad
      let speed = Math.hypot(ball.vx, ball.vy);
      let newDirX = Math.sin(angle);
      let newDirY = -Math.cos(angle);
      let norm = Math.hypot(newDirX, newDirY);
      if(norm > 0) {
        newDirX /= norm;
        newDirY /= norm;
      }
      ball.vx = newDirX * Math.min(speed, 5.8);
      ball.vy = newDirY * Math.min(speed, 5.8);
      if(ball.vy > -0.5) ball.vy = -2.8; // ensure upward bounce
      // push ball slightly above paddle
      ball.y = paddle.y - ball.r - 1;
    }
  }
  
  function handleBumperCollision() {
    for(let i = 0; i < bumpers.length; i++) {
      const b = bumpers[i];
      const dx = ball.x - b.x;
      const dy = ball.y - b.y;
      const dist = Math.hypot(dx, dy);
      const minDist = ball.r + b.r;
      if(dist < minDist) {
        // collision response: reflect velocity
        const angle = Math.atan2(dy, dx);
        const normX = Math.cos(angle);
        const normY = Math.sin(angle);
        const velDotN = ball.vx * normX + ball.vy * normY;
        if(velDotN < 0) {
          const bounce = 1.05;
          ball.vx = (ball.vx - 2 * velDotN * normX) * bounce;
          ball.vy = (ball.vy - 2 * velDotN * normY) * bounce;
        }
        // reposition outside bumper
        const overlap = minDist - dist;
        ball.x += normX * overlap;
        ball.y += normY * overlap;
        score += 10;
        updateUI();
        // small spark style effect - just update once per collision
      }
    }
  }
  
  // mouse move for paddle
  let mouseX = width/2;
  function movePaddle(e) {
    const rect = canvas.getBoundingClientRect();
    const scaleX = canvas.width / rect.width;
    let mouseCanvasX = (e.clientX - rect.left) * scaleX;
    mouseCanvasX = Math.min(Math.max(mouseCanvasX, 0), width);
    mouseX = mouseCanvasX;
  }
  canvas.addEventListener('mousemove', movePaddle);
  canvas.addEventListener('touchmove', (e) => {
    e.preventDefault();
    const rect = canvas.getBoundingClientRect();
    const touch = e.touches[0];
    let touchX = (touch.clientX - rect.left) * (canvas.width/rect.width);
    touchX = Math.min(Math.max(touchX, 0), width);
    mouseX = touchX;
  });
  
  function updatePaddlePosition() {
    paddle.x = mouseX - paddle.w/2;
    paddle.x = Math.min(Math.max(paddle.x, 0), width - paddle.w);
  }
  
  // game loop
  let animationId = null;
  function gameUpdate() {
    if(!gameActive) return;
    updatePaddlePosition();
    
    // move ball
    ball.x += ball.vx;
    ball.y += ball.vy;
    
    // wall collisions (might trigger lose life)
    const lost = handleWallCollision();
    if(lost) {
      // ball was reset in loseLife, ensure position
      if(ball.y + ball.r >= height + 10) ball.y = height - 50;
    }
    
    handlePaddleCollision();
    handleBumperCollision();
    
    // small boundary security
    ball.x = Math.min(Math.max(ball.x, ball.r), width - ball.r);
    ball.y = Math.min(Math.max(ball.y, ball.r), height - ball.r);
    // extra check: ball stuck in ceiling zone? fine
    
    // drawing everything
    drawCanvas();
    animationId = requestAnimationFrame(gameUpdate);
  }
  
  function drawCanvas() {
    ctx.clearRect(0, 0, width, height);
    // fluffy background with dots
    ctx.fillStyle = "#fef3ea";
    ctx.fillRect(0, 0, width, height);
    for(let i=0; i<80; i++) {
      ctx.beginPath();
      ctx.arc( (i*17)%width, (i*9)%height, 1, 0, Math.PI*2);
      ctx.fillStyle = "#ffd9c4";
      ctx.fill();
    }
    
    // draw bumpers (cute pastel)
    for(let b of bumpers) {
      ctx.beginPath();
      ctx.arc(b.x, b.y, b.r-1, 0, Math.PI*2);
      ctx.fillStyle = "#ffba91";
      ctx.fill();
      ctx.beginPath();
      ctx.arc(b.x, b.y, b.r-3, 0, Math.PI*2);
      ctx.fillStyle = "#ffdbbc";
      ctx.fill();
      ctx.beginPath();
      ctx.arc(b.x, b.y, b.r-5, 0, Math.PI*2);
      ctx.fillStyle = "#fec6a0";
      ctx.fill();
      ctx.fillStyle = "#c26a46";
      ctx.font = "bold 12px monospace";
      ctx.fillText("⚡", b.x-6, b.y+5);
    }
    
    // paddle (cute rounded)
    ctx.shadowBlur = 0;
    ctx.fillStyle = "#e07c5c";
    ctx.beginPath();
    ctx.roundRect(paddle.x, paddle.y, paddle.w, paddle.h, 12);
    ctx.fill();
    ctx.fillStyle = "#b24626";
    ctx.beginPath();
    ctx.roundRect(paddle.x+4, paddle.y-2, paddle.w-8, 5, 4);
    ctx.fill();
    
    // ball: little bouncing star
    ctx.beginPath();
    ctx.arc(ball.x, ball.y, ball.r, 0, Math.PI*2);
    ctx.fillStyle = "#ff8866";
    ctx.fill();
    ctx.beginPath();
    ctx.arc(ball.x-1, ball.y-1, 1.5, 0, Math.PI*2);
    ctx.fillStyle = "white";
    ctx.fill();
    ctx.fillStyle = "#aa5135";
    ctx.beginPath();
    ctx.arc(ball.x+1, ball.y+1, 1, 0, Math.PI*2);
    ctx.fill();
    
    // little stars
    ctx.fillStyle = "#f5bc8e";
    for(let s=0; s<3; s++) {
      ctx.fillRect(ball.x-3 + s*3, ball.y-4, 1, 1);
    }
    ctx.fillStyle = "#ab6e52";
    ctx.font = "bold 18px monospace";
    ctx.fillText("✦", ball.x-4, ball.y-3);
    
    // extra wall glow
    ctx.strokeStyle = "#ffcfb0";
    ctx.lineWidth = 1.5;
    ctx.strokeRect(5,5, width-10, height-10);
  }
  
  // helper canvas rounding
  if (!CanvasRenderingContext2D.prototype.roundRect) {
    CanvasRenderingContext2D.prototype.roundRect = function(x, y, w, h, r) {
      if (w < 2 * r) r = w / 2;
      if (h < 2 * r) r = h / 2;
      this.moveTo(x+r, y);
      this.lineTo(x+w-r, y);
      this.quadraticCurveTo(x+w, y, x+w, y+r);
      this.lineTo(x+w, y+h-r);
      this.quadraticCurveTo(x+w, y+h, x+w-r, y+h);
      this.lineTo(x+r, y+h);
      this.quadraticCurveTo(x, y+h, x, y+h-r);
      this.lineTo(x, y+r);
      this.quadraticCurveTo(x, y, x+r, y);
      return this;
    };
  }
  
  // reset event on window resize / orientation maintain canvas dimensions
  function resizeCanvasDisplay() {
    // canvas CSS adapt but actual pixels fixed 400x400, no content loss
  }
  window.addEventListener('resize', () => {});
  
  // start game
  gameUpdate();
  updateUI();
  
  // initial reset so game is alive
  resetBall();
  
  // little floating emoji addition: make initial orbit angles lively
  for(let i=0;i<angles.length;i++) angles[i] = orbits[i].angle + i*0.7;
  
  // also ensure that we don't break game if ball stuck, set small occasional push 
  setInterval(() => {
    if(ball && (ball.vx === 0 && ball.vy === 0)) {
      ball.vx = (Math.random() - 0.5)*3;
      ball.vy = -2.5;
    }
    // safety respawn if ball stuck above paddle for too long
    if(ball && ball.y + ball.r > height - 5 && ball.vy > -0.2) {
      ball.vy = -3;
    }
  }, 1500);
  
  // Cursor fun effect on canvas
  canvas.style.cursor = "grab";
</script>
</body>
</html>
