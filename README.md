<svg width="860" height="180" viewBox="0 0 860 180" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0f0c29"/>
      <stop offset="50%" style="stop-color:#1a1040"/>
      <stop offset="100%" style="stop-color:#24243e"/>
    </linearGradient>
    <linearGradient id="lineGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#6c47ff;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#00d4ff;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#7b2ff7;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="fillGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#6c47ff;stop-opacity:0.25"/>
      <stop offset="100%" style="stop-color:#6c47ff;stop-opacity:0"/>
    </linearGradient>
    <linearGradient id="line2Grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00d4ff;stop-opacity:0.4"/>
      <stop offset="100%" style="stop-color:#00d4ff;stop-opacity:0.1"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="2.5" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="softGlow">
      <feGaussianBlur stdDeviation="4" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="860" height="180" fill="url(#bgGrad)"/>

  <!-- Subtle grid lines -->
  <line x1="0" y1="40" x2="860" y2="40" stroke="#ffffff" stroke-opacity="0.04" stroke-width="1"/>
  <line x1="0" y1="80" x2="860" y2="80" stroke="#ffffff" stroke-opacity="0.04" stroke-width="1"/>
  <line x1="0" y1="120" x2="860" y2="120" stroke="#ffffff" stroke-opacity="0.04" stroke-width="1"/>
  <line x1="0" y1="160" x2="860" y2="160" stroke="#ffffff" stroke-opacity="0.04" stroke-width="1"/>
  <line x1="86" y1="0" x2="86" y2="180" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="172" y1="0" x2="172" y2="180" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="258" y1="0" x2="258" y2="180" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="344" y1="0" x2="344" y2="180" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="430" y1="0" x2="430" y2="180" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="516" y1="0" x2="516" y2="180" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="602" y1="0" x2="602" y2="180" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="688" y1="0" x2="688" y2="180" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>
  <line x1="774" y1="0" x2="774" y2="180" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1"/>

  <!-- Secondary dim line (behind) -->
  <polyline
    points="0,130 60,120 110,135 160,115 200,125 240,100 290,110 340,90 380,105 420,85 460,95 500,70 540,82 580,65 620,78 660,55 700,68 740,50 790,60 860,45"
    fill="none"
    stroke="url(#line2Grad)"
    stroke-width="1.5"
    stroke-linejoin="round"
  />

  <!-- Fill area under main line -->
  <polygon
    points="0,180 0,125 50,110 100,120 150,100 190,112 230,88 280,98 330,78 370,92 410,72 450,84 495,58 540,70 580,54 620,67 660,44 700,57 745,39 800,50 860,36 860,180"
    fill="url(#fillGrad)"
  />

  <!-- Main glowing line -->
  <polyline
    points="0,125 50,110 100,120 150,100 190,112 230,88 280,98 330,78 370,92 410,72 450,84 495,58 540,70 580,54 620,67 660,44 700,57 745,39 800,50 860,36"
    fill="none"
    stroke="url(#lineGrad)"
    stroke-width="2.5"
    stroke-linejoin="round"
    filter="url(#glow)"
  />

  <!-- Data point dots -->
  <circle cx="230" cy="88" r="3.5" fill="#6c47ff" filter="url(#glow)"/>
  <circle cx="330" cy="78" r="3.5" fill="#00d4ff" filter="url(#glow)"/>
  <circle cx="495" cy="58" r="4" fill="#00d4ff" filter="url(#softGlow)"/>
  <circle cx="660" cy="44" r="3.5" fill="#6c47ff" filter="url(#glow)"/>
  <circle cx="800" cy="50" r="3" fill="#7b2ff7" filter="url(#glow)"/>

  <!-- Tooltip bubble on peak -->
  <rect x="468" y="28" width="56" height="22" rx="5" fill="#6c47ff" fill-opacity="0.85"/>
  <text x="496" y="43" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" fill="white">+42.7%</text>

  <!-- Name text -->
  <text x="430" y="90" text-anchor="middle" font-family="'Segoe UI', 'Arial', sans-serif" font-size="26" font-weight="700" fill="white" filter="url(#softGlow)">John Carlo Dizon</text>

  <!-- Subtitle -->
  <text x="430" y="113" text-anchor="middle" font-family="'Courier New', monospace" font-size="12" fill="#a0a8c0" letter-spacing="1">Backend Developer · Desktop Dev · Philippines</text>

</svg>
