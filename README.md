<!-- ═══════════════════════════════════════════════════════════════════
     PAREEK CYBER ACADEMY — README.md
     SVG-powered · 3D perspective · mobile-first · single-file platform
     ═══════════════════════════════════════════════════════════════════ -->

<div align="center">

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 340" width="100%" style="max-width:900px;">
  <defs>
    <radialGradient id="heroBg" cx="50%" cy="40%" r="70%">
      <stop offset="0%" stop-color="#0a1a2e"/>
      <stop offset="55%" stop-color="#050b18"/>
      <stop offset="100%" stop-color="#02040a"/>
    </radialGradient>
    <linearGradient id="cyanGrad" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#22d3ee"/>
      <stop offset="100%" stop-color="#0891b2"/>
    </linearGradient>
    <linearGradient id="violetGrad" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#a855f7"/>
      <stop offset="100%" stop-color="#7c3aed"/>
    </linearGradient>
    <linearGradient id="greenGrad" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#22c55e"/>
      <stop offset="100%" stop-color="#16a34a"/>
    </linearGradient>
    <linearGradient id="titleGrad" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#22d3ee"/>
      <stop offset="50%" stop-color="#e0f2fe"/>
      <stop offset="100%" stop-color="#a855f7"/>
    </linearGradient>
    <linearGradient id="gridFade" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#22d3ee" stop-opacity="0"/>
      <stop offset="60%" stop-color="#22d3ee" stop-opacity="0.6"/>
      <stop offset="100%" stop-color="#22d3ee" stop-opacity="0.15"/>
    </linearGradient>
    <linearGradient id="floorFade" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#a855f7" stop-opacity="0.35"/>
      <stop offset="100%" stop-color="#22d3ee" stop-opacity="0"/>
    </linearGradient>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="glowStrong" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="8" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <rect width="900" height="340" fill="url(#heroBg)"/>
  <ellipse cx="450" cy="330" rx="520" ry="80" fill="url(#floorFade)"/>

  <!-- perspective grid floor -->
  <g opacity="0.35">
    <line x1="450" y1="235" x2="-200" y2="340" stroke="#22d3ee" stroke-width="0.6"/>
    <line x1="450" y1="235" x2="0" y2="340" stroke="#22d3ee" stroke-width="0.6"/>
    <line x1="450" y1="235" x2="200" y2="340" stroke="#22d3ee" stroke-width="0.6"/>
    <line x1="450" y1="235" x2="400" y2="340" stroke="#22d3ee" stroke-width="0.6"/>
    <line x1="450" y1="235" x2="500" y2="340" stroke="#22d3ee" stroke-width="0.6"/>
    <line x1="450" y1="235" x2="700" y2="340" stroke="#22d3ee" stroke-width="0.6"/>
    <line x1="450" y1="235" x2="900" y2="340" stroke="#22d3ee" stroke-width="0.6"/>
    <line x1="450" y1="235" x2="1100" y2="340" stroke="#22d3ee" stroke-width="0.6"/>
  </g>
  <g opacity="0.28" fill="none" stroke="#a855f7" stroke-width="0.5">
    <path d="M -100 250 Q 450 215 1000 250"/>
    <path d="M -100 270 Q 450 235 1000 270"/>
    <path d="M -100 295 Q 450 260 1000 295"/>
    <path d="M -100 320 Q 450 285 1000 320"/>
  </g>

  <!-- floating nodes -->
  <g filter="url(#glow)">
    <circle cx="140" cy="90" r="3" fill="#22d3ee"/>
    <circle cx="230" cy="60" r="2.5" fill="#a855f7"/>
    <circle cx="760" cy="80" r="3" fill="#22d3ee"/>
    <circle cx="820" cy="150" r="2.5" fill="#a855f7"/>
    <circle cx="80" cy="180" r="2" fill="#22c55e"/>
    <circle cx="830" cy="220" r="2" fill="#22d3ee"/>
  </g>
  <g stroke="#22d3ee" stroke-width="0.4" opacity="0.5">
    <line x1="140" y1="90" x2="230" y2="60"/>
    <line x1="760" y1="80" x2="820" y2="150"/>
  </g>

  <!-- central shield / core -->
  <g transform="translate(450,150)" filter="url(#glowStrong)">
    <polygon points="0,-90 70,-50 70,40 0,90 -70,40 -70,-50" fill="none" stroke="url(#cyanGrad)" stroke-width="2.5"/>
    <polygon points="0,-70 54,-38 54,30 0,70 -54,30 -54,-38" fill="none" stroke="url(#violetGrad)" stroke-width="1.2" opacity="0.7"/>
    <path d="M -22 6 L -6 22 L 26 -18" fill="none" stroke="#22c55e" stroke-width="6" stroke-linecap="round" stroke-linejoin="round"/>
  </g>

  <!-- orbiting nodes around core -->
  <g opacity="0.9">
    <ellipse cx="450" cy="150" rx="170" ry="42" fill="none" stroke="#22d3ee" stroke-width="0.8" opacity="0.5" transform="rotate(-14 450 150)"/>
    <ellipse cx="450" cy="150" rx="210" ry="52" fill="none" stroke="#a855f7" stroke-width="0.6" opacity="0.4" transform="rotate(18 450 150)"/>
    <circle cx="270" cy="130" r="3.5" fill="#22d3ee" filter="url(#glow)"/>
    <circle cx="640" cy="180" r="3.5" fill="#a855f7" filter="url(#glow)"/>
  </g>

  <!-- title -->
  <text x="450" y="62" text-anchor="middle" font-family="Orbitron,Segoe UI,sans-serif" font-size="30" font-weight="900" letter-spacing="3" fill="url(#titleGrad)">PAREEK CYBER ACADEMY</text>
  <text x="450" y="92" text-anchor="middle" font-family="JetBrains Mono,Courier New,monospace" font-size="12" letter-spacing="8" fill="#67e8f9" opacity="0.85">L E A R N   ·   B U I L D   ·   B R E A K   ·   D E F E N D</text>

  <!-- subtitle -->
  <text x="450" y="272" text-anchor="middle" font-family="Segoe UI,sans-serif" font-size="12.5" fill="#94a3b8">Browser-native cybersecurity academy · 33-level roadmap · 250+ topics · 100+ original CTF challenges</text>
  <text x="450" y="292" text-anchor="middle" font-family="JetBrains Mono,Courier New,monospace" font-size="10.5" letter-spacing="2" fill="#64748b">ONE FILE · NO BACKEND · NO TRACKING · GITHUB PAGES READY</text>

  <!-- corner HUD marks -->
  <g opacity="0.6" stroke="#22d3ee" stroke-width="1.2" fill="none">
    <path d="M 20 20 L 20 40 M 20 20 L 40 20"/>
    <path d="M 880 20 L 880 40 M 880 20 L 860 20"/>
    <path d="M 20 320 L 20 300 M 20 320 L 40 320"/>
    <path d="M 880 320 L 880 300 M 880 320 L 860 320"/>
  </g>
</svg>

<br/>

[![Live](https://img.shields.io/badge/🚀_LIVE_ACADEMY-ENTER_THE_CYBER_WORLD-22d3ee?style=for-the-badge&labelColor=0a1628)](#-github-pages-deployment)
[![Roadmap](https://img.shields.io/badge/🧭_ROADMAP-33_LEVELS-a855f7?style=for-the-badge&labelColor=0a1628)](#-the-a-z-cybersecurity-roadmap)
[![CTF](https://img.shields.io/badge/⚡_CTF-100+_CHALLENGES-22c55e?style=for-the-badge&labelColor=0a1628)](#-cyber-ctf--the-arena)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-181717?style=flat-square&logo=github&logoColor=white)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Education-22d3ee?style=flat-square)
![CTF](https://img.shields.io/badge/CTF-Original-a855f7?style=flat-square)
![Education](https://img.shields.io/badge/Education-Open-22c55e?style=flat-square)
![Open Source](https://img.shields.io/badge/Open_Source-Educational-f59e0b?style=flat-square)

</div>

---

## ⚡ SYSTEM BOOT

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 200" width="100%" style="max-width:900px;">
  <defs>
    <linearGradient id="bootBg" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#050b18"/>
      <stop offset="100%" stop-color="#02040a"/>
    </linearGradient>
    <filter id="bootGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>
  <rect width="900" height="200" rx="12" fill="url(#bootBg)" stroke="#22d3ee" stroke-opacity="0.35"/>
  <rect x="0" y="0" width="900" height="28" rx="12" fill="#0a1a2e" opacity="0.8"/>
  <circle cx="20" cy="14" r="5" fill="#ef4444"/>
  <circle cx="38" cy="14" r="5" fill="#f59e0b"/>
  <circle cx="56" cy="14" r="5" fill="#22c55e"/>
  <text x="80" y="18" font-family="JetBrains Mono,monospace" font-size="11" fill="#64748b">pca@academy:~$ ./boot --secure</text>

  <g font-family="JetBrains Mono,monospace" font-size="13" fill="#9fe8ff">
    <text x="24" y="60" fill="#22d3ee">▸</text>
    <text x="44" y="60">SYSTEM INITIALIZING</text>
    <text x="780" y="60" fill="#22c55e">[ OK ]</text>

    <text x="24" y="86" fill="#22d3ee">▸</text>
    <text x="44" y="86">CYBER LEARNING ENVIRONMENT ONLINE</text>
    <text x="780" y="86" fill="#22c55e">[ OK ]</text>

    <text x="24" y="112" fill="#22d3ee">▸</text>
    <text x="44" y="112">3D COMMAND CENTER ACTIVE</text>
    <text x="780" y="112" fill="#22c55e">[ OK ]</text>

    <text x="24" y="138" fill="#22d3ee">▸</text>
    <text x="44" y="138">CTF / LAB / SECURITY ENGINEERING MODULES LOADED</text>
    <text x="780" y="138" fill="#22c55e">[ OK ]</text>

    <text x="24" y="176" fill="#22c55e" filter="url(#bootGlow)">▸ WELCOME, RECRUIT. THE COMMAND CENTER IS YOURS.</text>
  </g>
</svg>

---

## 🎯 What Is PAREEK CYBER ACADEMY?

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 220" width="100%" style="max-width:900px;">
  <defs>
    <linearGradient id="panelG" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0a1a2e" stop-opacity="0.95"/>
      <stop offset="100%" stop-color="#0f0a1f" stop-opacity="0.95"/>
    </linearGradient>
    <linearGradient id="panelEdge" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#22d3ee" stop-opacity="0.9"/>
      <stop offset="100%" stop-color="#a855f7" stop-opacity="0.5"/>
    </linearGradient>
  </defs>

  <!-- isometric-ish panel -->
  <polygon points="40,30 860,30 880,50 880,200 60,200 40,180" fill="url(#panelG)" stroke="url(#panelEdge)" stroke-width="1.5"/>
  <polygon points="40,30 60,50 880,50 860,30" fill="#22d3ee" opacity="0.15"/>
  <polygon points="40,30 40,180 60,200 60,50" fill="#22d3ee" opacity="0.1"/>

  <text x="60" y="72" font-family="Orbitron,sans-serif" font-size="14" font-weight="700" fill="#22d3ee" letter-spacing="3">▸ MISSION BRIEF</text>

  <text x="60" y="102" font-family="Segoe UI,sans-serif" font-size="13" fill="#cbd5e1">
    A complete, browser-native cybersecurity learning environment — shipped as one
  </text>
  <text x="60" y="122" font-family="Segoe UI,sans-serif" font-size="13" fill="#cbd5e1">
    self-contained index.html file. No backend. No database. No build step. No tracking.
  </text>
  <text x="60" y="142" font-family="Segoe UI,sans-serif" font-size="13" fill="#cbd5e1">
    3D cyber interface, 33-level roadmap, 250+ topics, interactive labs, terminal
  </text>
  <text x="60" y="162" font-family="Segoe UI,sans-serif" font-size="13" fill="#cbd5e1">
    simulator, and an original browser-based CTF engine — all inside one file.
  </text>

  <text x="60" y="188" font-family="JetBrains Mono,monospace" font-size="11" fill="#22c55e" letter-spacing="1">▸ ETHICAL USE ONLY · AUTHORIZED LABS · ORIGINAL CONTENT</text>
</svg>

### ▸ Who It Is For

| Audience | What You Get |
|---|---|
| **Absolute beginners** | A structured path from "what is a CPU" to cloud security architecture |
| **Self-taught learners** | Ordered curriculum with prerequisites — no scattered tutorials |
| **Students** | A portfolio-ready platform to demonstrate real, practical skill |
| **Professionals pivoting** | Deep dives into SOC, DFIR, cloud, DevSecOps, AI security |
| **Educators** | A ready-to-fork teaching environment for workshops |
| **CTF newcomers** | 100+ original, safe simulated challenges with hints |

### ▸ Why It Exists

Most cybersecurity learning is scattered and disconnected from practice. This platform gives learners a **single ordered path** — where every topic has prerequisites, every level has labs, and every concept has a defensive counterpoint. Theory without practice decays. Practice without theory is fragile. This platform enforces both.

---

## 🧭 THE A–Z CYBERSECURITY ROADMAP

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 1120" width="100%" style="max-width:900px;">
  <defs>
    <linearGradient id="rmBg" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#050b18"/>
      <stop offset="100%" stop-color="#0a0518"/>
    </linearGradient>
    <linearGradient id="pathG" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#22d3ee"/>
      <stop offset="50%" stop-color="#a855f7"/>
      <stop offset="100%" stop-color="#22c55e"/>
    </linearGradient>
    <radialGradient id="nodeG">
      <stop offset="0%" stop-color="#22d3ee"/>
      <stop offset="100%" stop-color="#0a1628"/>
    </radialGradient>
    <filter id="rmGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <rect width="900" height="1120" rx="14" fill="url(#rmBg)" stroke="#22d3ee" stroke-opacity="0.25"/>

  <!-- central glowing path -->
  <path d="M 450 50 L 450 1080" stroke="url(#pathG)" stroke-width="4" fill="none" opacity="0.55" filter="url(#rmGlow)"/>
  <path d="M 450 50 L 450 1080" stroke="url(#pathG)" stroke-width="1.5" fill="none"/>

  <!-- level marker function-like rows -->
  <g font-family="Orbitron,sans-serif" font-size="13" font-weight="700" fill="#e2e8f0">

    <!-- L0 -->
    <circle cx="450" cy="70" r="10" fill="url(#nodeG)" stroke="#22d3ee" stroke-width="2" filter="url(#rmGlow)"/>
    <rect x="480" y="55" width="360" height="34" rx="8" fill="#0a1a2e" stroke="#22d3ee" stroke-opacity="0.6"/>
    <text x="500" y="77" fill="#67e8f9" font-family="JetBrains Mono,monospace" font-size="11">L00</text>
    <text x="545" y="77" font-size="12">Computer Fundamentals</text>

    <!-- L1 -->
    <circle cx="450" cy="110" r="8" fill="#0a1628" stroke="#22d3ee" stroke-width="2"/>
    <rect x="480" y="95" width="360" height="30" rx="8" fill="#081524" stroke="#22d3ee" stroke-opacity="0.4"/>
    <text x="500" y="115" fill="#67e8f9" font-family="JetBrains Mono,monospace" font-size="11">L01</text>
    <text x="545" y="115" font-size="12">Linux</text>

    <!-- L2 -->
    <circle cx="450" cy="150" r="8" fill="#0a1628" stroke="#22d3ee" stroke-width="2"/>
    <rect x="480" y="135" width="360" height="30" rx="8" fill="#081524" stroke="#22d3ee" stroke-opacity="0.4"/>
    <text x="500" y="155" fill="#67e8f9" font-family="JetBrains Mono,monospace" font-size="11">L02</text>
    <text x="545" y="155" font-size="12">Networking</text>

    <!-- L3 -->
    <circle cx="450" cy="190" r="8" fill="#0a1628" stroke="#22d3ee" stroke-width="2"/>
    <rect x="480" y="175" width="360" height="30" rx="8" fill="#081524" stroke="#22d3ee" stroke-opacity="0.4"/>
    <text x="500" y="195" fill="#67e8f9" font-family="JetBrains Mono,monospace" font-size="11">L03</text>
    <text x="545" y="195" font-size="12">Python for Cybersecurity</text>

    <!-- L4 -->
    <circle cx="450" cy="230" r="8" fill="#0a1628" stroke="#22d3ee" stroke-width="2"/>
    <rect x="480" y="215" width="360" height="30" rx="8" fill="#081524" stroke="#22d3ee" stroke-opacity="0.4"/>
    <text x="500" y="235" fill="#67e8f9" font-family="JetBrains Mono,monospace" font-size="11">L04</text>
    <text x="545" y="235" font-size="12">Web Technologies</text>

    <!-- L5 -->
    <circle cx="450" cy="270" r="8" fill="#0a1628" stroke="#0891b2" stroke-width="2"/>
    <rect x="480" y="255" width="360" height="30" rx="8" fill="#081524" stroke="#0891b2" stroke-opacity="0.5"/>
    <text x="500" y="275" fill="#67e8f9" font-family="JetBrains Mono,monospace" font-size="11">L05</text>
    <text x="545" y="275" font-size="12">Cybersecurity Fundamentals</text>

    <!-- L6 -->
    <circle cx="450" cy="310" r="8" fill="#0a1628" stroke="#7c3aed" stroke-width="2"/>
    <rect x="480" y="295" width="360" height="30" rx="8" fill="#0f0a1f" stroke="#7c3aed" stroke-opacity="0.5"/>
    <text x="500" y="315" fill="#c4b5fd" font-family="JetBrains Mono,monospace" font-size="11">L06</text>
    <text x="545" y="315" font-size="12">Cryptography</text>

    <!-- L7 -->
    <circle cx="450" cy="350" r="8" fill="#0a1628" stroke="#7c3aed" stroke-width="2"/>
    <rect x="480" y="335" width="360" height="30" rx="8" fill="#0f0a1f" stroke="#7c3aed" stroke-opacity="0.5"/>
    <text x="500" y="355" fill="#c4b5fd" font-family="JetBrains Mono,monospace" font-size="11">L07</text>
    <text x="545" y="355" font-size="12">Web Security</text>

    <!-- L8 -->
    <circle cx="450" cy="390" r="8" fill="#0a1628" stroke="#7c3aed" stroke-width="2"/>
    <rect x="480" y="375" width="360" height="30" rx="8" fill="#0f0a1f" stroke="#7c3aed" stroke-opacity="0.5"/>
    <text x="500" y="395" fill="#c4b5fd" font-family="JetBrains Mono,monospace" font-size="11">L08</text>
    <text x="545" y="395" font-size="12">API Security</text>

    <!-- L9 -->
    <circle cx="450" cy="430" r="8" fill="#0a1628" stroke="#7c3aed" stroke-width="2"/>
    <rect x="480" y="415" width="360" height="30" rx="8" fill="#0f0a1f" stroke="#7c3aed" stroke-opacity="0.5"/>
    <text x="500" y="435" fill="#c4b5fd" font-family="JetBrains Mono,monospace" font-size="11">L09</text>
    <text x="545" y="435" font-size="12">Operating System Security</text>

    <!-- L10 -->
    <circle cx="450" cy="470" r="8" fill="#0a1628" stroke="#7c3aed" stroke-width="2"/>
    <rect x="480" y="455" width="360" height="30" rx="8" fill="#0f0a1f" stroke="#7c3aed" stroke-opacity="0.5"/>
    <text x="500" y="475" fill="#c4b5fd" font-family="JetBrains Mono,monospace" font-size="11">L10</text>
    <text x="545" y="475" font-size="12">Active Directory Security</text>

    <!-- L11 -->
    <circle cx="450" cy="510" r="8" fill="#0a1628" stroke="#a855f7" stroke-width="2"/>
    <rect x="480" y="495" width="360" height="30" rx="8" fill="#12091f" stroke="#a855f7" stroke-opacity="0.55"/>
    <text x="500" y="515" fill="#d8b4fe" font-family="JetBrains Mono,monospace" font-size="11">L11</text>
    <text x="545" y="515" font-size="12">Cloud Computing</text>

    <!-- L12 -->
    <circle cx="450" cy="550" r="8" fill="#0a1628" stroke="#a855f7" stroke-width="2"/>
    <rect x="480" y="535" width="360" height="30" rx="8" fill="#12091f" stroke="#a855f7" stroke-opacity="0.55"/>
    <text x="500" y="555" fill="#d8b4fe" font-family="JetBrains Mono,monospace" font-size="11">L12</text>
    <text x="545" y="555" font-size="12">Cloud Security</text>

    <!-- L13 -->
    <circle cx="450" cy="590" r="8" fill="#0a1628" stroke="#a855f7" stroke-width="2"/>
    <rect x="480" y="575" width="360" height="30" rx="8" fill="#12091f" stroke="#a855f7" stroke-opacity="0.55"/>
    <text x="500" y="595" fill="#d8b4fe" font-family="JetBrains Mono,monospace" font-size="11">L13</text>
    <text x="545" y="595" font-size="12">DevSecOps</text>

    <!-- L14 -->
    <circle cx="450" cy="630" r="8" fill="#0a1628" stroke="#ec4899" stroke-width="2"/>
    <rect x="480" y="615" width="360" height="30" rx="8" fill="#1a0a1f" stroke="#ec4899" stroke-opacity="0.55"/>
    <text x="500" y="635" fill="#f9a8d4" font-family="JetBrains Mono,monospace" font-size="11">L14</text>
    <text x="545" y="635" font-size="12">SOC Operations</text>

    <!-- L15 -->
    <circle cx="450" cy="670" r="8" fill="#0a1628" stroke="#ec4899" stroke-width="2"/>
    <rect x="480" y="655" width="360" height="30" rx="8" fill="#1a0a1f" stroke="#ec4899" stroke-opacity="0.55"/>
    <text x="500" y="675" fill="#f9a8d4" font-family="JetBrains Mono,monospace" font-size="11">L15</text>
    <text x="545" y="675" font-size="12">SIEM &amp; Detection</text>

    <!-- L16 -->
    <circle cx="450" cy="710" r="8" fill="#0a1628" stroke="#ec4899" stroke-width="2"/>
    <rect x="480" y="695" width="360" height="30" rx="8" fill="#1a0a1f" stroke="
