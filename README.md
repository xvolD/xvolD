<div align="center" style="background-color: #0a0a0a; padding: 20px; border-radius: 10px; color: #aaa; font-family: 'Courier New', monospace;">

<!-- Animated Gothic Banner (no emoji, pure SVG) -->
<svg width="100%" height="300" viewBox="0 0 800 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
    <filter id="intenseGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="8" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
    <radialGradient id="moonGrad" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#fff5e6" />
      <stop offset="70%" stop-color="#d9c8a9" />
      <stop offset="100%" stop-color="#8b7355" />
    </radialGradient>
    <linearGradient id="fogGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#2d1b3d" stop-opacity="0.3" />
      <stop offset="100%" stop-color="#2d1b3d" stop-opacity="0" />
    </linearGradient>
    <path id="bat" d="M0,10 Q5,0 10,5 Q15,0 20,10 Q15,8 10,12 Q5,8 0,10 Z" fill="#1a0a1a" />
    <rect id="candle" x="-6" y="0" width="12" height="40" fill="#3a2a2a" rx="2" />
    <ellipse id="candle-top" cx="0" cy="0" rx="6" ry="2" fill="#4a3a3a" />
    <path id="wick" d="M0,-2 Q1,-6 2,-8" stroke="#333" stroke-width="1.5" fill="none" />
  </defs>

  <rect width="800" height="300" fill="#0a0a0a" />
  
  <!-- Moon -->
  <circle cx="650" cy="80" r="50" fill="url(#moonGrad)" opacity="0.8">
    <animate attributeName="opacity" values="0.7;1;0.7" dur="4s" repeatCount="indefinite" />
  </circle>
  <circle cx="650" cy="80" r="60" fill="none" stroke="#8b7355" stroke-width="2" opacity="0.3">
    <animate attributeName="r" values="60;70;60" dur="4s" repeatCount="indefinite" />
    <animate attributeName="opacity" values="0.2;0.5;0.2" dur="4s" repeatCount="indefinite" />
  </circle>

  <!-- Cathedral -->
  <path d="M0,300 L0,260 L20,260 L20,220 L30,220 L30,260 L50,260 L50,210 L60,210 L60,260 L80,260 L80,230 L90,230 L90,260 L110,260 L110,190 L120,190 L120,260 L140,260 L140,250 L150,250 L150,260 L170,260 L170,200 L185,200 L185,260 L200,260 L200,240 L210,240 L210,260 L230,260 L230,180 L250,180 L250,260 L270,260 L270,220 L285,220 L285,260 L300,260 L300,240 L310,240 L310,260 L330,260 L330,210 L350,210 L350,260 L370,260 L370,230 L385,230 L385,260 L400,260 L400,190 L420,190 L420,260 L440,260 L440,250 L450,250 L450,260 L470,260 L470,200 L485,200 L485,260 L500,260 L500,240 L510,240 L510,260 L530,260 L530,180 L550,180 L550,260 L570,260 L570,220 L585,220 L585,260 L600,260 L600,240 L610,240 L610,260 L630,260 L630,210 L650,210 L650,260 L670,260 L670,230 L685,230 L685,260 L700,260 L700,250 L710,250 L710,260 L730,260 L730,190 L750,190 L750,260 L770,260 L770,220 L785,220 L785,260 L800,260 L800,300 Z" fill="#150f1a" opacity="0.9" />
  
  <!-- Windows (glowing purple) -->
  <circle cx="60" cy="220" r="4" fill="#800080" opacity="0.8">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite" />
  </circle>
  <circle cx="350" cy="210" r="4" fill="#800080" opacity="0.8">
    <animate attributeName="opacity" values="0.6;1;0.6" dur="2.5s" repeatCount="indefinite" begin="0.5s" />
  </circle>
  <circle cx="550" cy="180" r="4" fill="#800080" opacity="0.8">
    <animate attributeName="opacity" values="0.4;0.9;0.4" dur="3.5s" repeatCount="indefinite" begin="1s" />
  </circle>

  <!-- Fog -->
  <ellipse cx="200" cy="270" rx="150" ry="20" fill="url(#fogGrad)">
    <animateTransform attributeName="transform" type="translate" values="0,0;100,0;0,0" dur="20s" repeatCount="indefinite" />
  </ellipse>
  <ellipse cx="500" cy="260" rx="180" ry="25" fill="url(#fogGrad)">
    <animateTransform attributeName="transform" type="translate" values="0,0;-80,0;0,0" dur="25s" repeatCount="indefinite" />
  </ellipse>
  <ellipse cx="700" cy="280" rx="140" ry="18" fill="url(#fogGrad)">
    <animateTransform attributeName="transform" type="translate" values="0,0;60,0;0,0" dur="18s" repeatCount="indefinite" />
  </ellipse>

  <!-- Bats -->
  <use href="#bat" x="250" y="60" transform="scale(0.8)">
    <animateTransform attributeName="transform" type="translate" values="0,0;20,-10;0,0" dur="6s" repeatCount="indefinite" />
    <animateTransform attributeName="transform" type="scale" values="0.8;0.9;0.8" dur="0.3s" repeatCount="indefinite" additive="sum" />
  </use>
  <use href="#bat" x="400" y="100" transform="scale(0.6) scale(-1,1)">
    <animateTransform attributeName="transform" type="translate" values="0,0;-15,-5;0,0" dur="7s" repeatCount="indefinite" />
    <animateTransform attributeName="transform" type="scale" values="0.6;0.7;0.6" dur="0.25s" repeatCount="indefinite" additive="sum" />
  </use>
  <use href="#bat" x="150" y="120" transform="scale(0.5)">
    <animateTransform attributeName="transform" type="translate" values="0,0;10,5;0,0" dur="5s" repeatCount="indefinite" />
    <animateTransform attributeName="transform" type="scale" values="0.5;0.55;0.5" dur="0.35s" repeatCount="indefinite" additive="sum" />
  </use>

  <!-- Candle -->
  <g transform="translate(150, 230)">
    <use href="#candle" />
    <use href="#candle-top" />
    <use href="#wick" />
    <path d="M-3,-10 Q0,-18 3,-10 Q2,-8 0,-8 Q-2,-8 -3,-10 Z" fill="#ff8c00">
      <animate attributeName="d" values="M-3,-10 Q0,-18 3,-10 Q2,-8 0,-8 Q-2,-8 -3,-10 Z;M-2.5,-9 Q0,-17 2.5,-9 Q1.5,-7 0,-7 Q-1.5,-7 -2.5,-9 Z;M-3,-10 Q0,-18 3,-10 Q2,-8 0,-8 Q-2,-8 -3,-10 Z" dur="0.2s" repeatCount="indefinite" />
      <animate attributeName="opacity" values="0.8;1;0.8" dur="0.15s" repeatCount="indefinite" />
    </path>
    <circle cx="0" cy="-12" r="10" fill="#ff8c00" opacity="0.2">
      <animate attributeName="r" values="10;12;10" dur="0.2s" repeatCount="indefinite" />
      <animate attributeName="opacity" values="0.1;0.3;0.1" dur="0.2s" repeatCount="indefinite" />
    </circle>
  </g>

  <!-- Glitch title -->
  <g filter="url(#intenseGlow)">
    <text x="400" y="140" text-anchor="middle" font-size="80" font-family="monospace" fill="#FF00FF" opacity="0.8">
      xvolD
      <animate attributeName="opacity" values="0;0.8;0;0;0.8;0" dur="2s" repeatCount="indefinite" keyTimes="0;0.1;0.2;0.7;0.8;1" />
      <animateTransform attributeName="transform" type="translate" values="0,0;-3,-2;0,0;0,0;-3,2;0,0" dur="2s" repeatCount="indefinite" keyTimes="0;0.1;0.2;0.7;0.8;1" additive="sum" />
    </text>
    <text x="400" y="140" text-anchor="middle" font-size="80" font-family="monospace" fill="#00ffff" opacity="0.8">
      xvolD
      <animate attributeName="opacity" values="0;0;0.8;0;0;0.8;0" dur="2s" repeatCount="indefinite" keyTimes="0;0.1;0.15;0.25;0.7;0.75;1" />
      <animateTransform attributeName="transform" type="translate" values="0,0;0,0;2,1;0,0;0,0;-2,-1;0,0" dur="2s" repeatCount="indefinite" keyTimes="0;0.1;0.15;0.25;0.7;0.75;1" additive="sum" />
    </text>
    <text x="400" y="140" text-anchor="middle" font-size="80" font-family="monospace" fill="#e0e0e0">
      xvolD
      <animate attributeName="opacity" values="1;1;0.9;1;1;0.9;1" dur="2s" repeatCount="indefinite" />
    </text>
  </g>

  <!-- Subtitle -->
  <text x="400" y="180" text-anchor="middle" font-size="22" font-family="monospace" fill="#800080" opacity="0.9">
    <animate attributeName="opacity" values="0.3;1;0.3" dur="3s" repeatCount="indefinite" />
    Enter the Abyss
  </text>

  <!-- Particles -->
  <circle cx="100" cy="150" r="1.5" fill="#800080">
    <animate attributeName="cy" values="150;130;150" dur="6s" repeatCount="indefinite" />
    <animate attributeName="opacity" values="0;1;0" dur="6s" repeatCount="indefinite" />
  </circle>
  <circle cx="300" cy="180" r="1" fill="#FF00FF">
    <animate attributeName="cy" values="180;160;180" dur="5s" repeatCount="indefinite" begin="1s" />
    <animate attributeName="opacity" values="0;1;0" dur="5s" repeatCount="indefinite" begin="1s" />
  </circle>
  <circle cx="550" cy="120" r="1.5" fill="#DDA0DD">
    <animate attributeName="cy" values="120;100;120" dur="7s" repeatCount="indefinite" begin="2s" />
    <animate attributeName="opacity" values="0;1;0" dur="7s" repeatCount="indefinite" begin="2s" />
  </circle>
  <circle cx="700" cy="160" r="1" fill="#800080">
    <animate attributeName="cy" values="160;140;160" dur="4.5s" repeatCount="indefinite" begin="0.5s" />
    <animate attributeName="opacity" values="0;1;0" dur="4.5s" repeatCount="indefinite" begin="0.5s" />
  </circle>
</svg>

<br>

<!-- About -->
<h2 style="color: #800080; letter-spacing: 2px;">About the Entity</h2>
<p style="max-width: 600px; margin: auto; color: #ccc; font-size: 16px; line-height: 1.6;">
  Welcome, wanderer... I am <strong style="color: #FF00FF;">xvolD</strong>, a denizen of the digital shadows.<br>
  Code necromancer, architect of the arcane, weaving spells in silicon and logic.<br>
  By candlelight I craft my grimories of software, ever seeking the next forbidden commit.
</p>

<br>

<!-- Grimoire -->
<h2 style="color: #800080; letter-spacing: 2px;">Grimoire of Skills</h2>
<p style="color: #aaa;">Languages and tools I commune with:</p>
<img src="https://img.shields.io/badge/Python-000000?style=for-the-badge&logo=python&logoColor=purple&labelColor=0a0a0a&color=800080" />
<img src="https://img.shields.io/badge/JavaScript-000000?style=for-the-badge&logo=javascript&logoColor=purple&labelColor=0a0a0a&color=800080" />
<img src="https://img.shields.io/badge/C++-000000?style=for-the-badge&logo=cplusplus&logoColor=purple&labelColor=0a0a0a&color=800080" />
<br>
<img src="https://img.shields.io/badge/Docker-000000?style=for-the-badge&logo=docker&logoColor=purple&labelColor=0a0a0a&color=800080" />
<img src="https://img.shields.io/badge/Linux-000000?style=for-the-badge&logo=linux&logoColor=purple&labelColor=0a0a0a&color=800080" />
<img src="https://img.shields.io/badge/Git-000000?style=for-the-badge&logo=git&logoColor=purple&labelColor=0a0a0a&color=800080" />

<br><br>

<!-- Stats -->
<h2 style="color: #800080; letter-spacing: 2px;">Stats & Curses</h2>
<div style="display: flex; justify-content: center; gap: 10px; flex-wrap: wrap;">
  <img height="150" src="https://github-readme-stats.vercel.app/api?username=xvolD&show_icons=true&theme=dark&title_color=800080&text_color=ccc&icon_color=800080&bg_color=0d1117&hide_border=true&count_private=true" />
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=xvolD&layout=compact&theme=dark&title_color=800080&text_color=ccc&bg_color=0d1117&hide_border=true" />
</div>

<br>

<!-- Counter (without emoji in the link, just text) -->
<img src="https://komarev.com/ghpvc/?username=xvolD&style=flat-square&color=800080&label=Souls+Witnessed" />

<br><br>

<!-- Prophecy -->
<details style="color: #aaa; max-width: 600px; margin: auto;">
  <summary style="color: #800080; font-size: 18px; cursor: pointer;">Unveil the Prophecy...</summary>
  <br>
  <p style="font-style: italic; background: #111; padding: 15px; border-left: 3px solid #800080; border-radius: 0 8px 8px 0;">
    "In the digital void, whispers of code become eternal.<br>
    From the depths of the terminal, xvolD rises, cloaked in shadow and semicolons.<br>
    The stars align, the repositories awaken... prepare for the pull request of destiny."
  </p>
</details>

<br>

<!-- Summon -->
<h2 style="color: #800080; letter-spacing: 2px;">Summon Me</h2>
<a href="https://github.com/xvolD"><img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=purple&labelColor=0a0a0a&color=800080" /></a>
<a href="#"><img src="https://img.shields.io/badge/Email-800080?style=for-the-badge&logo=gmail&logoColor=black&labelColor=0a0a0a&color=800080" /></a>

<br><br>
<p style="font-size: 12px; color: #555;">«What is dead may never die, but rises again, harder and stronger.»</p>

</div>