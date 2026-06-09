<div align="center">

<!-- BANNER -->
<img src="./assets/banner.png" alt="VoidX3D Banner" width="100%">

<br>

<!-- ============================================ -->
<!--           EPIC ANIMATED SVG HEADER            -->
<!-- ============================================ -->
<svg width="100%" height="380" viewBox="0 0 1000 380" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d1117;stop-opacity:1" />
      <stop offset="30%" style="stop-color:#0a1628;stop-opacity:1" />
      <stop offset="70%" style="stop-color:#0d1117;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#0a1929;stop-opacity:1" />
    </linearGradient>
    <linearGradient id="glowGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00D9FF;stop-opacity:0" />
      <stop offset="50%" style="stop-color:#00D9FF;stop-opacity:0.9" />
      <stop offset="100%" style="stop-color:#00D9FF;stop-opacity:0" />
    </linearGradient>
    <linearGradient id="titleGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00D9FF" />
      <stop offset="30%" style="stop-color:#00E5FF" />
      <stop offset="50%" style="stop-color:#8A2BE2" />
      <stop offset="70%" style="stop-color:#FF6B6B" />
      <stop offset="100%" style="stop-color:#FFD93D" />
    </linearGradient>
    <linearGradient id="wave1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00D9FF;stop-opacity:0.12" />
      <stop offset="50%" style="stop-color:#8A2BE2;stop-opacity:0.12" />
      <stop offset="100%" style="stop-color:#FF6B6B;stop-opacity:0.12" />
    </linearGradient>
    <linearGradient id="wave2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#FF6B6B;stop-opacity:0.08" />
      <stop offset="50%" style="stop-color:#00D9FF;stop-opacity:0.08" />
      <stop offset="100%" style="stop-color:#8A2BE2;stop-opacity:0.08" />
    </linearGradient>
    <linearGradient id="wave3" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#FFD93D;stop-opacity:0.06" />
      <stop offset="50%" style="stop-color:#00D9FF;stop-opacity:0.06" />
      <stop offset="100%" style="stop-color:#FF6B6B;stop-opacity:0.06" />
    </linearGradient>
    <radialGradient id="glowCircle" cx="50%" cy="50%" r="50%">
      <stop offset="0%" style="stop-color:#00D9FF;stop-opacity:0.08" />
      <stop offset="100%" style="stop-color:#00D9FF;stop-opacity:0" />
    </radialGradient>
    <filter id="titleGlow">
      <feGaussianBlur stdDeviation="8" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="softGlow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#00D9FF" stroke-width="0.3" opacity="0.05"/>
    </pattern>
  </defs>

  <!-- Background with grid -->
  <rect width="1000" height="380" fill="url(#bgGrad)" rx="15"/>
  <rect width="1000" height="380" fill="url(#grid)" rx="15"/>

  <!-- Ambient glow circle behind title -->
  <circle cx="500" cy="140" r="200" fill="url(#glowCircle)">
    <animate attributeName="r" values="180;220;180" dur="4s" repeatCount="indefinite"/>
  </circle>

  <!-- Animated wave 1 (deep) -->
  <path fill="url(#wave1)">
    <animate attributeName="d" dur="14s" repeatCount="indefinite"
      values="M0,300 Q125,260 250,280 T500,260 T750,280 T1000,260 L1000,380 L0,380 Z;
              M0,300 Q125,280 250,260 T500,280 T750,260 T1000,280 L1000,380 L0,380 Z;
              M0,300 Q125,260 250,280 T500,260 T750,280 T1000,260 L1000,380 L0,380 Z"/>
  </path>

  <!-- Animated wave 2 (mid) -->
  <path fill="url(#wave2)">
    <animate attributeName="d" dur="11s" repeatCount="indefinite"
      values="M0,320 Q150,290 300,310 T600,290 T900,310 L1000,300 L1000,380 L0,380 Z;
              M0,320 Q150,310 300,290 T600,310 T900,290 L1000,300 L1000,380 L0,380 Z;
              M0,320 Q150,290 300,310 T600,290 T900,310 L1000,300 L1000,380 L0,380 Z"/>
  </path>

  <!-- Animated wave 3 (shallow) -->
  <path fill="url(#wave3)">
    <animate attributeName="d" dur="8s" repeatCount="indefinite"
      values="M0,340 Q100,320 200,335 T400,320 T600,335 T800,320 T1000,335 L1000,380 L0,380 Z;
              M0,340 Q100,335 200,320 T400,335 T600,320 T800,335 T1000,320 L1000,380 L0,380 Z;
              M0,340 Q100,320 200,335 T400,320 T600,335 T800,320 T1000,335 L1000,380 L0,380 Z"/>
  </path>

  <!-- Floating particles layer 1 -->
  <circle cx="80" cy="60" r="2.5" fill="#00D9FF" opacity="0.7">
    <animate attributeName="cy" from="-10" to="380" dur="7s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.7;0.1;0.7" dur="3.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="200" cy="100" r="1.5" fill="#8A2BE2" opacity="0.6">
    <animate attributeName="cy" from="-10" to="380" dur="10s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0.1;0.6" dur="4s" repeatCount="indefinite"/>
  </circle>
  <circle cx="350" cy="40" r="2" fill="#FF6B6B" opacity="0.5">
    <animate attributeName="cy" from="-10" to="380" dur="9s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;0.1;0.5" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="500" cy="130" r="3" fill="#FFD93D" opacity="0.4">
    <animate attributeName="cy" from="-10" to="380" dur="12s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;0.1;0.4" dur="5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="650" cy="70" r="1.8" fill="#00D9FF" opacity="0.6">
    <animate attributeName="cy" from="-10" to="380" dur="8.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0.1;0.6" dur="3.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="780" cy="110" r="2.2" fill="#8A2BE2" opacity="0.5">
    <animate attributeName="cy" from="-10" to="380" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;0.1;0.5" dur="4.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="920" cy="50" r="1.5" fill="#FF6B6B" opacity="0.7">
    <animate attributeName="cy" from="-10" to="380" dur="11s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.7;0.1;0.7" dur="2.5s" repeatCount="indefinite"/>
  </circle>

  <!-- Floating particles layer 2 (smaller, slower) -->
  <circle cx="130" cy="90" r="1" fill="#00D9FF" opacity="0.3">
    <animate attributeName="cy" from="-10" to="380" dur="15s" repeatCount="indefinite"/>
  </circle>
  <circle cx="430" cy="30" r="1.2" fill="#FFD93D" opacity="0.3">
    <animate attributeName="cy" from="-10" to="380" dur="18s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="150" r="1" fill="#8A2BE2" opacity="0.3">
    <animate attributeName="cy" from="-10" to="380" dur="13s" repeatCount="indefinite"/>
  </circle>

  <!-- Rotating hexagon 1 -->
  <g transform="translate(150, 210)" opacity="0.12">
    <animateTransform attributeName="transform" type="rotate" from="0 150 210" to="360 150 210" dur="30s" repeatCount="indefinite"/>
    <polygon points="0,-25 21.7,-12.5 21.7,12.5 0,25 -21.7,12.5 -21.7,-12.5" fill="none" stroke="#00D9FF" stroke-width="1.5"/>
  </g>

  <!-- Rotating hexagon 2 -->
  <g transform="translate(850, 200)" opacity="0.10">
    <animateTransform attributeName="transform" type="rotate" from="360 850 200" to="0 850 200" dur="35s" repeatCount="indefinite"/>
    <polygon points="0,-18 15.6,-9 15.6,9 0,18 -15.6,9 -15.6,-9" fill="none" stroke="#8A2BE2" stroke-width="1.5"/>
  </g>

  <!-- Orbiting ring -->
  <ellipse cx="500" cy="290" rx="350" ry="20" fill="none" stroke="#00D9FF" stroke-width="0.5" opacity="0.08">
    <animate attributeName="ry" values="20;25;20" dur="6s" repeatCount="indefinite"/>
  </ellipse>

  <!-- Orbiting satellite -->
  <circle r="3" fill="#8A2BE2" opacity="0.6" filter="url(#softGlow)">
    <animateMotion dur="12s" repeatCount="indefinite"
      path="M150,290 Q500,270 850,290 Q500,310 150,290"/>
  </circle>

  <!-- Code rain effect (right side) -->
  <g opacity="0.06" font-family="monospace" font-size="10" fill="#00D9FF">
    <text x="860" y="100">&lt;/&gt;</text>
    <text x="890" y="140">const</text>
    <text x="870" y="180">=&gt;</text>
    <text x="900" y="220">{ }</text>
    <text x="880" y="260">fn</text>
    <text x="850" y="300">async</text>
  </g>

  <!-- Code rain effect (left side) -->
  <g opacity="0.06" font-family="monospace" font-size="10" fill="#8A2BE2">
    <text x="80" y="120">import</text>
    <text x="60" y="160">class</text>
    <text x="90" y="200">new</text>
    <text x="70" y="240">this</text>
    <text x="100" y="280">=&gt;</text>
    <text x="80" y="320">yield</text>
  </g>

  <!-- Glowing line under title -->
  <rect x="200" y="225" width="600" height="2" fill="url(#glowGrad)" rx="1" opacity="0.8">
    <animate attributeName="opacity" values="0.3;0.9;0.3" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="width" values="600;650;600" dur="5s" repeatCount="indefinite"/>
  </rect>

  <!-- Main title -->
  <text x="500" y="120" text-anchor="middle" fill="url(#titleGrad)" font-size="82" font-weight="900" font-family="'Segoe UI', -apple-system, Arial, sans-serif" filter="url(#titleGlow)" letter-spacing="3">
    VoidX3D
    <animate attributeName="opacity" values="1;0.85;1" dur="3s" repeatCount="indefinite"/>
  </text>

  <!-- Subtitle with gradient -->
  <text x="500" y="175" text-anchor="middle" fill="#8b949e" font-size="17" font-family="'Courier New', monospace" letter-spacing="5">
    <tspan fill="#00D9FF" font-weight="bold">FULL STACK</tspan>
    <tspan fill="#8b949e"> DEVELOPER </tspan>
    <tspan fill="#8A2BE2">✦</tspan>
    <tspan fill="#8b949e"> BACKEND ENGINEER </tspan>
    <tspan fill="#FF6B6B">✦</tspan>
    <tspan fill="#8b949e"> AI BUILDER</tspan>
  </text>

  <!-- Tech stack marquee line -->
  <g opacity="0.4">
    <text x="500" y="200" text-anchor="middle" fill="#484f58" font-size="11" font-family="'Courier New', monospace" letter-spacing="8">
      TS • JS • PY • GO • RS • KT • Java • C++ • C# • Swift
    </text>
  </g>

  <!-- Tagline -->
  <text x="500" y="260" text-anchor="middle" fill="#484f58" font-size="13" font-family="'Courier New', monospace" letter-spacing="2">
    Building production-ready systems • Creating AI-powered tools • Shipping what matters
  </text>

  <!-- Location / meta pill -->
  <g transform="translate(340, 290)">
    <rect x="0" y="0" width="320" height="34" rx="17" fill="#161b22" stroke="#30363d" stroke-width="1"/>
    <text x="160" y="22" text-anchor="middle" fill="#8b949e" font-size="13" font-family="'Courier New', monospace">
      🇳🇵 Pokhara, Nepal  •  17 y/o  •  3+ Years  •  Self-Taught
    </text>
  </g>
</svg>

<br>

<!-- ============================================ -->
<!--           ANIMATED TYPING SVG                -->
<!-- ============================================ -->
<p>
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=00D9FF&center=true&vCenter=true&multiline=true&repeat=true&width=900&height=120&lines=%E2%9A%A1+Building+Production-Ready+Systems;%F0%9F%8E%AE+Creating+AI-Powered+Tools+%26+APIs;%F0%9F%94%A5+Shipping+Real+Projects+That+Matter;%E2%9A%94%EF%B8%8F+Bleach+Fan+%26+Code+Warrior;%F0%9F%9A%80+Self-Taught+Developer+%7C+Always+Learning;%F0%9F%92%BB+Full+Stack+%7C+Backend+%7C+AI+%7C+Mobile+%7C+DevOps" alt="Typing SVG" />
</p>

<!-- ============================================ -->
<!--           BADGES BAR                        -->
<!-- ============================================ -->
<p>
  <a href="https://github.com/VoidX3D"><img src="https://img.shields.io/badge/Profile_Views-2.8K+-blueviolet?style=for-the-badge&logo=eye&logoColor=white" alt="views"/></a>
  <a href="https://github.com/VoidX3D?tab=followers"><img src="https://img.shields.io/github/followers/VoidX3D?label=Followers&style=for-the-badge&logo=github&logoColor=white&color=blue" alt="followers"/></a>
  <a href="https://github.com/VoidX3D?tab=repositories"><img src="https://img.shields.io/badge/Repos-23+-orange?style=for-the-badge&logo=github&logoColor=white" alt="repos"/></a>
  <a href="https://github.com/VoidX3D"><img src="https://img.shields.io/badge/Focus-Backend_%26_AI-red?style=for-the-badge&logo=robot&logoColor=white" alt="focus"/></a>
  <a href="https://github.com/VoidX3D/VoidX3D"><img src="https://img.shields.io/badge/Status-Shipping_%F0%9F%9A%80-success?style=for-the-badge&logoColor=white" alt="status"/></a>
  <a href="https://github.com/sponsors/VoidX3D"><img src="https://img.shields.io/badge/Sponsor-EA4AAA?style=for-the-badge&logo=github-sponsors&logoColor=white" alt="sponsor"/></a>
</p>

<!-- VISITOR COUNTER -->
<p>
  <img src="https://visitcount.itsvg.in/api?id=voidx3d&icon=5&color=6" alt="Visit Count"/>
  <img src="https://img.shields.io/github/stars/VoidX3D?style=for-the-badge&logo=github&logoColor=white&color=yellow" alt="GitHub Stars"/>
  <img src="https://img.shields.io/badge/Made%20in-Nepal-DF2A2A?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAAbwAAAG8B8aLcQwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAEoSURBVDiNpZMxTsNAEEX/rNeOAwUlHVdA4gJcAokLUNDRcAQkLkCBaOgouQIVFQ0XQKJwA0oqCqSA+7HBWjuOHWKTkWb1dj6zfwT/gV4+mPefBQBmZkVVx4h8KOYLAkBE3kppV1VHjS4i2yLSV9UjACLyDgBmdo+IewD4UtVrM3tzzpcAgIiIiNwyM1VtmNkbMx8BwDOAzwhCBHAXQggAcGZmL875awBAVS+ZOWMMAHDOGQDAzJ+Z+YmZ7wEgxngCAAhCi8xs/xeYOTLnWgCAEAIAYIyxiDHeOOdORKQTY+wCQOsPIITAInJsZksAICKDlNJpSqkfY5yKyBQAJkJ/CyEEETEHYGZ2oao3InIIAPnXcyJyy8xHAFBE2hhjJ6W0BwBnZvZ3Ii4AH2b20Gq1vgHyNFk+bSdMxQAAAABJRU5ErkJggg==&logoColor=white" alt="Made in Nepal"/>
</p>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%">

</div>

---

<!-- ============================================ -->
<!--              ABOUT ME                        -->
<!-- ============================================ -->
<div align="center">

# ⚡ About Me

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

</div>

<table align="center">
  <tr>
    <td width="60%" valign="top">

**Hey! I'm VoidX3D** — a 17-year-old **Full Stack Developer & Backend Engineer** from Pokhara, Nepal 🇳🇵. With 3+ years of self-taught experience, I'm on a mission to build production-ready systems, engineer AI-powered APIs, and ship real projects that matter.

My coding journey started at **age 12 with HTML/CSS**, building my first calculator. Since then, it's been a non-stop grind across 14+ languages, countless frameworks, and a growing collection of shipped projects — from Android music players to anime tracking platforms, admin dashboards to streaming APIs.

**My philosophy:** "*Code with passion, debug with patience, deploy with pride!*" Every bug is a lesson, every project is progress. Just like Ichigo's journey in Bleach — always pushing limits, never giving up. ⚔️

```typescript
const voidx3d = {
  name: "VoidX3D",
  role: "Full Stack Developer & Backend Engineer",
  location: "Pokhara, Nepal 🇳🇵",
  pronouns: "he/him",
  age: 17,
  experience: "3+ years self-taught",
  code: ["TypeScript", "JavaScript", "Python", "Kotlin", "Java", "Go", "Rust"],
  architect: ["Microservices", "Event-Driven", "RESTful APIs", "System Design"],
  tools: ["Node.js", "React", "Next.js", "Docker", "K8s", "Supabase", "Redis"],
  ai_ml: ["TensorFlow", "PyTorch", "OpenCV", "LangChain", "OpenAI"],
  philosophy: {
    code: "Clean architecture > Quick hacks",
    learning: "Build projects, not just tutorials",
    shipping: "Done is better than perfect, but iterate toward excellence",
    mindset: "Every bug is a lesson, every project is progress"
  },
  motivation: "Code with passion, debug with patience, deploy with pride! 🚀"
};
```

    </td>
    <td width="40%" valign="top">

### 📋 Personal

| Attribute | Detail |
|-----------|--------|
| **Name** | VoidX3D |
| **Role** | Full Stack Dev & Backend Engineer |
| **Location** | Pokhara, Gandaki, Nepal 🇳🇵 |
| **Education** | @ Motherland Secondary School |
| **Age** | 17 |
| **Experience** | 3+ Years Self-Taught |
| **Time Zone** | UTC+5:45 (yes, really!) |

### 🎯 Current Focus

- Backend Architecture & System Design
- AI/ML Integration into Production Apps
- Real-time Applications & APIs
- Performance Optimization
- Open Source Contributions

### 📚 Learning

- Microservices & Event-Driven Architecture
- Cloud Native (K8s, Serverless)
- Machine Learning Ops
- Blockchain & Web3
- Game Engine Development

### ⚔️ Interests

- Watching Anime (Bleach is peak!)
- Building Side Projects
- Gaming & Game Dev
- Writing Technical Blogs
- Long walks with Himalayan views 🏔️

### 🎵 Coding Vibe

- **Music:** Lo-fi + Anime OSTs
- **Time:** 10 PM – 3 AM 🦉
- **Fuel:** Coffee ☕ (essential)
- **Theme:** Dark mode only 💀

    </td>
  </tr>
</table>

<details>
<summary><b>🎯 2026 Goals & Roadmap</b></summary>
<br>

<div align="center">

| Quarter | Focus | Key Objectives |
|:-------:|:------|:---------------|
| **Q1** 🎄 | **Foundation** | Master TypeScript, System Design patterns, Microservices architecture |
| **Q2** ❄️ | **Growth** | Cloud cert prep, ML deployment pipelines, CI/CD mastery |
| **Q3** 🎁 | **Execution** | Launch AI SaaS platform, 100+ OSS contributions, Tech blog series |
| **Q4** ⛄ | **Mastery** | Scale existing projects, WebAssembly deep-dive, Game engine development |

</div>

</details>

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%">

---

<!-- ============================================ -->
<!--              TECH STACK                      -->
<!-- ============================================ -->
<div align="center">

# 🛠️ Tech Stack

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

My complete arsenal — all **57 icons hosted locally** in this repo.

</div>

### 💻 Programming Languages

<div align="center">
  <table>
    <tr>
      <td align="center" width="96"><img src="assets/icons/javascript.svg" width="48" height="48" alt="JS"/><br><b>JavaScript</b></td>
      <td align="center" width="96"><img src="assets/icons/typescript.svg" width="48" height="48" alt="TS"/><br><b>TypeScript</b></td>
      <td align="center" width="96"><img src="assets/icons/python.svg" width="48" height="48" alt="Python"/><br><b>Python</b></td>
      <td align="center" width="96"><img src="assets/icons/java.svg" width="48" height="48" alt="Java"/><br><b>Java</b></td>
      <td align="center" width="96"><img src="assets/icons/cplusplus.svg" width="48" height="48" alt="C++"/><br><b>C++</b></td>
      <td align="center" width="96"><img src="assets/icons/csharp.svg" width="48" height="48" alt="C#"/><br><b>C#</b></td>
      <td align="center" width="96"><img src="assets/icons/go.svg" width="48" height="48" alt="Go"/><br><b>Go</b></td>
    </tr>
    <tr>
      <td align="center" width="96"><img src="assets/icons/kotlin.svg" width="48" height="48" alt="Kotlin"/><br><b>Kotlin</b></td>
      <td align="center" width="96"><img src="assets/icons/swift.svg" width="48" height="48" alt="Swift"/><br><b>Swift</b></td>
      <td align="center" width="96"><img src="assets/icons/php.svg" width="48" height="48" alt="PHP"/><br><b>PHP</b></td>
      <td align="center" width="96"><img src="assets/icons/rust.svg" width="48" height="48" alt="Rust"/><br><b>Rust</b></td>
      <td align="center" width="96"><img src="assets/icons/html5.svg" width="48" height="48" alt="HTML"/><br><b>HTML5</b></td>
      <td align="center" width="96"><img src="assets/icons/css3.svg" width="48" height="48" alt="CSS"/><br><b>CSS3</b></td>
      <td align="center" width="96"><img src="assets/icons/bash.svg" width="48" height="48" alt="Bash"/><br><b>Bash</b></td>
    </tr>
  </table>
</div>

### 🎨 Frontend

<div align="center">
  <table>
    <tr>
      <td align="center" width="96"><img src="assets/icons/react.svg" width="48" height="48" alt="React"/><br><b>React</b></td>
      <td align="center" width="96"><img src="assets/icons/nextjs.svg" width="48" height="48" alt="Next"/><br><b>Next.js</b></td>
      <td align="center" width="96"><img src="assets/icons/vuejs.svg" width="48" height="48" alt="Vue"/><br><b>Vue.js</b></td>
      <td align="center" width="96"><img src="assets/icons/svelte.svg" width="48" height="48" alt="Svelte"/><br><b>Svelte</b></td>
      <td align="center" width="96"><img src="assets/icons/tailwindcss.svg" width="48" height="48" alt="Tailwind"/><br><b>Tailwind</b></td>
      <td align="center" width="96"><img src="assets/icons/bootstrap.svg" width="48" height="48" alt="Bootstrap"/><br><b>Bootstrap</b></td>
      <td align="center" width="96"><img src="assets/icons/sass.svg" width="48" height="48" alt="Sass"/><br><b>Sass</b></td>
    </tr>
    <tr>
      <td align="center" width="96"><img src="assets/icons/materialui.svg" width="48" height="48" alt="MUI"/><br><b>MUI</b></td>
    </tr>
  </table>
</div>

### ⚙️ Backend & API

<div align="center">
  <table>
    <tr>
      <td align="center" width="96"><img src="assets/icons/nodejs.svg" width="48" height="48" alt="Node"/><br><b>Node.js</b></td>
      <td align="center" width="96"><img src="assets/icons/express.svg" width="48" height="48" alt="Express"/><br><b>Express</b></td>
      <td align="center" width="96"><img src="assets/icons/nestjs.svg" width="48" height="48" alt="NestJS"/><br><b>NestJS</b></td>
      <td align="center" width="96"><img src="assets/icons/fastapi.svg" width="48" height="48" alt="FastAPI"/><br><b>FastAPI</b></td>
      <td align="center" width="96"><img src="assets/icons/flask.svg" width="48" height="48" alt="Flask"/><br><b>Flask</b></td>
      <td align="center" width="96"><img src="assets/icons/django.svg" width="48" height="48" alt="Django"/><br><b>Django</b></td>
      <td align="center" width="96"><img src="assets/icons/spring.svg" width="48" height="48" alt="Spring"/><br><b>Spring</b></td>
    </tr>
  </table>
</div>

### 📱 Mobile & Cross-Platform

<div align="center">
  <table>
    <tr>
      <td align="center" width="96"><img src="assets/icons/react.svg" width="48" height="48" alt="RN"/><br><b>React Native</b></td>
      <td align="center" width="96"><img src="assets/icons/flutter.svg" width="48" height="48" alt="Flutter"/><br><b>Flutter</b></td>
      <td align="center" width="96"><img src="assets/icons/kotlin.svg" width="48" height="48" alt="Kotlin"/><br><b>Kotlin</b></td>
      <td align="center" width="96"><img src="assets/icons/swift.svg" width="48" height="48" alt="Swift"/><br><b>Swift</b></td>
      <td align="center" width="96"><img src="assets/icons/android.svg" width="48" height="48" alt="Android"/><br><b>Android</b></td>
      <td align="center" width="96"><img src="assets/icons/apple.svg" width="48" height="48" alt="iOS"/><br><b>iOS</b></td>
    </tr>
  </table>
</div>

### 🗄️ Databases & Storage

<div align="center">
  <table>
    <tr>
      <td align="center" width="96"><img src="assets/icons/mongodb.svg" width="48" height="48" alt="Mongo"/><br><b>MongoDB</b></td>
      <td align="center" width="96"><img src="assets/icons/postgresql.svg" width="48" height="48" alt="Postgres"/><br><b>PostgreSQL</b></td>
      <td align="center" width="96"><img src="assets/icons/mysql.svg" width="48" height="48" alt="MySQL"/><br><b>MySQL</b></td>
      <td align="center" width="96"><img src="assets/icons/redis.svg" width="48" height="48" alt="Redis"/><br><b>Redis</b></td>
      <td align="center" width="96"><img src="assets/icons/firebase.svg" width="48" height="48" alt="Firebase"/><br><b>Firebase</b></td>
      <td align="center" width="96"><img src="assets/icons/supabase.svg" width="48" height="48" alt="Supabase"/><br><b>Supabase</b></td>
      <td align="center" width="96"><img src="assets/icons/sqlite.svg" width="48" height="48" alt="SQLite"/><br><b>SQLite</b></td>
    </tr>
  </table>
</div>

### ☁️ DevOps, Cloud & CI/CD

<div align="center">
  <table>
    <tr>
      <td align="center" width="96"><img src="assets/icons/docker.svg" width="48" height="48" alt="Docker"/><br><b>Docker</b></td>
      <td align="center" width="96"><img src="assets/icons/kubernetes.svg" width="48" height="48" alt="K8s"/><br><b>Kubernetes</b></td>
      <td align="center" width="96"><img src="assets/icons/aws.svg" width="48" height="48" alt="AWS"/><br><b>AWS</b></td>
      <td align="center" width="96"><img src="assets/icons/azure.svg" width="48" height="48" alt="Azure"/><br><b>Azure</b></td>
      <td align="center" width="96"><img src="assets/icons/gcp.svg" width="48" height="48" alt="GCP"/><br><b>GCP</b></td>
      <td align="center" width="96"><img src="assets/icons/jenkins.svg" width="48" height="48" alt="Jenkins"/><br><b>Jenkins</b></td>
      <td align="center" width="96"><img src="assets/icons/nginx.svg" width="48" height="48" alt="Nginx"/><br><b>Nginx</b></td>
    </tr>
  </table>
</div>

### 🤖 AI, ML & Data Science

<div align="center">
  <table>
    <tr>
      <td align="center" width="96"><img src="assets/icons/tensorflow.svg" width="48" height="48" alt="TF"/><br><b>TensorFlow</b></td>
      <td align="center" width="96"><img src="assets/icons/pytorch.svg" width="48" height="48" alt="PyTorch"/><br><b>PyTorch</b></td>
      <td align="center" width="96"><img src="assets/icons/scikitlearn.svg" width="48" height="48" alt="SKL"/><br><b>Scikit-learn</b></td>
      <td align="center" width="96"><img src="assets/icons/opencv.svg" width="48" height="48" alt="OpenCV"/><br><b>OpenCV</b></td>
      <td align="center" width="96"><img src="assets/icons/pandas.svg" width="48" height="48" alt="Pandas"/><br><b>Pandas</b></td>
      <td align="center" width="96"><img src="assets/icons/numpy.svg" width="48" height="48" alt="NumPy"/><br><b>NumPy</b></td>
    </tr>
  </table>
</div>

### 🛠️ Tools, Editors & Environment

<div align="center">
  <table>
    <tr>
      <td align="center" width="96"><img src="assets/icons/git.svg" width="48" height="48" alt="Git"/><br><b>Git</b></td>
      <td align="center" width="96"><img src="assets/icons/github.svg" width="48" height="48" alt="GitHub"/><br><b>GitHub</b></td>
      <td align="center" width="96"><img src="assets/icons/vscode.svg" width="48" height="48" alt="VSCode"/><br><b>VS Code</b></td>
      <td align="center" width="96"><img src="assets/icons/linux.svg" width="48" height="48" alt="Linux"/><br><b>Linux</b></td>
      <td align="center" width="96"><img src="assets/icons/vim.svg" width="48" height="48" alt="Vim"/><br><b>Vim</b></td>
      <td align="center" width="96"><img src="assets/icons/figma.svg" width="48" height="48" alt="Figma"/><br><b>Figma</b></td>
      <td align="center" width="96"><img src="assets/icons/postman.svg" width="48" height="48" alt="Postman"/><br><b>Postman</b></td>
    </tr>
  </table>
</div>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%">

---

<!-- ============================================ -->
<!--          GITHUB STATISTICS                   -->
<!-- ============================================ -->
<div align="center">

# 📊 GitHub Statistics

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

Live analytics — real-time stats from my GitHub activity.

</div>

<div align="center">

<!-- ROW 1: Stats + Streak -->
<img width="49%" height="195px" src="https://github-readme-stats.vercel.app/api?username=voidx3d&show_icons=true&count_private=true&hide_border=true&title_color=00D9FF&icon_color=00D9FF&text_color=c9d1d9&bg_color=0d1117&include_all_commits=true&rank_icon=github&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage" alt="GitHub Stats" />

<img width="49%" height="195px" src="https://github-readme-streak-stats.herokuapp.com/?user=voidx3d&theme=dark&hide_border=true&background=0D1117&stroke=00D9FF&ring=00D9FF&fire=FF6B6B&currStreakLabel=FFFFFF" alt="GitHub Streak" />

<!-- ROW 2: Languages + WakaTime -->
<img width="49%" height="195px" src="https://github-readme-stats.vercel.app/api/top-langs/?username=voidx3d&layout=compact&hide_border=true&title_color=00D9FF&text_color=c9d1d9&bg_color=0d1117&langs_count=12&size_weight=0.5&count_weight=0.5" alt="Top Languages" />

<img width="49%" height="195px" src="https://github-readme-stats.vercel.app/api/wakatime?username=voidx3d&hide_border=true&title_color=00D9FF&text_color=c9d1d9&bg_color=0d1117&layout=compact&custom_title=Weekly%20Coding%20Activity" alt="WakaTime" />

<!-- PROFILE SUMMARY -->
<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=voidx3d&theme=tokyonight" alt="Profile Details"/>

<!-- DETAILED STAT CARDS -->
<img width="32%" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=voidx3d&theme=tokyonight" alt="Repos Per Language"/>
<img width="32%" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=voidx3d&theme=tokyonight" alt="Most Commit Language"/>
<img width="32%" src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=voidx3d&theme=tokyonight&utcOffset=5.75" alt="Productive Time"/>

</div>

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%">

---

<!-- ============================================ -->
<!--          ACHIEVEMENTS & TROPHIES              -->
<!-- ============================================ -->
<div align="center">

# 🏆 Achievements & Trophies

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

</div>

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=voidx3d&theme=tokyonight&no-frame=true&no-bg=false&margin-w=4&column=8" alt="Trophies"/>
</div>

<br>

<div align="center">

| 🎯 Milestone | 📊 Status | 🎁 Target | 🏅 Achievement |
|:------------|:----------|:----------|:--------------|
| **Total Commits** | ![](https://img.shields.io/badge/1000+-success?style=flat-square) | 2000+ by 2026 | 🌟 Code Warrior |
| **Public Repos** | ![](https://img.shields.io/badge/40+-blue?style=flat-square) | 100+ Quality | 🎁 Project Master |
| **GitHub Stars** | ![](https://img.shields.io/badge/Growing-orange?style=flat-square) | 1000+ Stars | ⭐ Community Loved |
| **Contributions** | ![](https://img.shields.io/badge/Active-brightgreen?style=flat-square) | Daily Commits | ❄️ Consistent Builder |
| **Languages** | ![](https://img.shields.io/badge/14+-purple?style=flat-square) | Master 18+ | 🎅 Polyglot Dev |
| **Followers** | ![](https://img.shields.io/badge/Growing-cyan?style=flat-square) | 500+ Network | 🤝 Community Leader |

</div>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%">

---

<!-- ============================================ -->
<!--          ALL PROJECTS                        -->
<!-- ============================================ -->
<div align="center">

# 🚀 All Projects

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

Every repository I've built — from AI-powered APIs to interactive games, mobile apps to developer tools.

</div>

### 🔥 Featured / Latest

<div align="center">

| Project | Description | Stack | Stars |
|:--------|:------------|:------|:-----:|
<!-- FEATURED_TABLE_START -->
| [**Anime-Tracker**](https://github.com/VoidX3D/Anime-Tracker) | A feature-rich anime tracking platform built with Next.js and Supabase, integrating AniList and MyAnimeList APIs with smart recommendations, dark mode, PWA support, and a sleek glassmorphism design. | TypeScript | ⭐3 |
| [**RU_Club_Website**](https://github.com/VoidX3D/RU_Club_Website) | Official website for Motherland RU Club — a student environmental squad from Pokhara, Nepal. Built with React, TypeScript, Supabase, and Tailwind CSS. | TypeScript | ⭐2 |
| [**RU_Admin_Site**](https://github.com/VoidX3D/RU_Admin_Site) | React 19 + TypeScript admin panel for RU Club Motherland. Manages missions, announcements, members, stats, partners, and contact submissions via Supabase. Vite + Tailwind CSS. | TypeScript | ⭐0 |
| [**DexDiary**](https://github.com/VoidX3D/DexDiary) | A personal diary/journal application built with modern web technologies. Track your thoughts, memories, and daily reflections. | Kotlin | ⭐0 |
| [**hianime-api**](https://github.com/VoidX3D/hianime-api) | Unofficial REST API wrapper for HiAnime.to. Scrape anime data, episodes, streaming links, and more. | TypeScript | ⭐0 |
<!-- FEATURED_TABLE_END -->

</div>

<br>

<!-- PROJECT CARDS -->
<div align="center">
<!-- FEATURED_CARDS_START -->
  <a href="https://github.com/VoidX3D/Anime-Tracker"><img src="https://github-readme-stats.vercel.app/api/pin/?username=VoidX3D&repo=Anime-Tracker&theme=tokyonight&hide_border=true&bg_color=0d1117" alt="Anime-Tracker"/></a>
  <a href="https://github.com/VoidX3D/RU_Club_Website"><img src="https://github-readme-stats.vercel.app/api/pin/?username=VoidX3D&repo=RU_Club_Website&theme=tokyonight&hide_border=true&bg_color=0d1117" alt="RU_Club_Website"/></a>
  <a href="https://github.com/VoidX3D/RU_Admin_Site"><img src="https://github-readme-stats.vercel.app/api/pin/?username=VoidX3D&repo=RU_Admin_Site&theme=tokyonight&hide_border=true&bg_color=0d1117" alt="RU_Admin_Site"/></a>
  <a href="https://github.com/VoidX3D/DexDiary"><img src="https://github-readme-stats.vercel.app/api/pin/?username=VoidX3D&repo=DexDiary&theme=tokyonight&hide_border=true&bg_color=0d1117" alt="DexDiary"/></a>
  <a href="https://github.com/VoidX3D/hianime-api"><img src="https://github-readme-stats.vercel.app/api/pin/?username=VoidX3D&repo=hianime-api&theme=tokyonight&hide_border=true&bg_color=0d1117" alt="hianime-api"/></a>
<!-- FEATURED_CARDS_END -->
</div>

<br>

<details>
<summary><b>🤖 AI & Backend Projects (6)</b></summary>
<br>

<div align="center">

| Project | Description | Stack |
|:--------|:------------|:------|
| [**AniList Real**](https://github.com/VoidX3D/anilist-real) | ML-based anime recommendation engine with real-time tracking & analytics | React, Node.js, MongoDB, ML |
| [**AniWatch API**](https://github.com/VoidX3D/aniwatch-api) | Production streaming API with Redis caching, rate limiting, Docker deployment | Node.js, Express, Redis, Docker |
| [**Proxy M3U8X**](https://github.com/VoidX3D/proxy-m3u8x) | HLS video proxy with intelligent load balancing, failover & CDN optimization | Node.js, Express, FFmpeg |
| [**ANIWAVE1**](https://github.com/VoidX3D/ANIWAVE1) | Anime streaming platform | JavaScript, Node.js |
| [**api.consumet.org**](https://github.com/VoidX3D/api.consumet.org) | Media information API (Consumet fork) | TypeScript, Node.js |
| [**voidx3d-api**](https://github.com/VoidX3D/voidx3d-api) | Personal backend API service | JavaScript, Node.js |

</div>

</details>

<details>
<summary><b>🎮 Interactive & Game Projects (3)</b></summary>
<br>

<div align="center">

| Project | Description | Stack |
|:--------|:------------|:------|
| [**Quest for the Core**](https://github.com/VoidX3D/quest-for-the-core) | Custom game engine with physics, pixel art & achievement system | JS, Canvas API |
| [**Chrome Game**](https://github.com/VoidX3D/chrome-game) | Browser extension game — offline, local storage, smooth animations | JS, Chrome API |
| [**Kahoot Clone**](https://github.com/VoidX3D/kahootClone) | Real-time multiplayer quiz with live leaderboards & custom creator | React, Socket.io, Node.js |

</div>

</details>

<details>
<summary><b>🌐 Web Development (6)</b></summary>
<br>

<div align="center">

| Project | Description | Stack |
|:--------|:------------|:------|
| [**Portfolio**](https://github.com/VoidX3D/Portfolio) | Personal portfolio — modern animations, fully responsive, blazing fast | Next.js, TailwindCSS, Framer |
| [**Ubuntu Web Sim**](https://github.com/VoidX3D/ubuntu.websimulation.desktop) | Full desktop environment in-browser — file system, terminal, authentic UI | HTML, CSS, JS |
| [**starpack**](https://github.com/VoidX3D/starpack) | Latest project — package manager/tooling | JavaScript |
| [**final**](https://github.com/VoidX3D/final) | Latest TypeScript project | TypeScript |
| [**Varkzen**](https://github.com/VoidX3D/Varkzen) | Web application project | JavaScript |
| [**myvarkzen**](https://github.com/VoidX3D/myvarkzen) | Varkzen variant | JavaScript |

</div>

</details>

<details>
<summary><b>📱 Mobile & Android (3)</b></summary>
<br>

<div align="center">

| Project | Description | Stack |
|:--------|:------------|:------|
| [**PixelPlayer**](https://github.com/VoidX3D/PixelPlayer) | Privacy-first Android music player — Material 3, offline, equalizer, casting | Kotlin, Material 3 |
| [**DexDiary**](https://github.com/VoidX3D/DexDiary) | Modern diary/journal app — track daily thoughts & memories | Kotlin |
| [**DexDiary-legacy**](https://github.com/VoidX3D/DexDiary-legacy) | Legacy version of DexDiary | Kotlin |

</div>

</details>

<details>
<summary><b>🎄 Holiday & Fun (6)</b></summary>
<br>

<div align="center">

| Project | Description | Stack |
|:--------|:------------|:------|
| [**Christms-Card**](https://github.com/VoidX3D/Christms-Card) | Interactive Christmas card — snowfall, music, animations | Vite, HTML, CSS, JS |
| [**Christmas-Card**](https://github.com/VoidX3D/Christmas-Card) | Festive digital Christmas card with holiday greetings | HTML, CSS, JS |
| [**Christmas-Card-Belgium**](https://github.com/VoidX3D/Christmas-Card-Belgium) | Belgium-themed Christmas card | HTML, CSS, JS |
| [**MyChristmasCard**](https://github.com/VoidX3D/MyChristmasCard) | Personal Christmas card project | HTML, CSS, JS |
| [**Happy-Bday-maya**](https://github.com/VoidX3D/Happy-Bday-maya) | Animated birthday card with interactive design | HTML, CSS, JS |
| [**christmas**](https://github.com/VoidX3D/christmas) | Latest Christmas-themed project | JavaScript |

</div>

</details>

<details>
<summary><b>🔧 Tools, Starters & Utilities (8)</b></summary>
<br>

<div align="center">

| Project | Description | Stack |
|:--------|:------------|:------|
| [**Password-Manager**](https://github.com/VoidX3D/Password-Manager) | Secure password management tool | JavaScript |
| [**clcalc**](https://github.com/VoidX3D/clcalc) | Command-line calculator utility | JavaScript |
| [**vite-react-template**](https://github.com/VoidX3D/vite-react-template) | Vite + React starter template | TS, Vite |
| [**nextjs-project-starter**](https://github.com/VoidX3D/nextjs-project-starter) | Next.js project starter | JavaScript |
| [**Backup**](https://github.com/VoidX3D/Backup) | Utility scripts, configs & automation backups | HTML, JS |
| [**player**](https://github.com/VoidX3D/player) | Media player application | JavaScript |
| [**player-sheet**](https://github.com/VoidX3D/player-sheet) | Player data sheet manager | JavaScript |
| [**NewSheetAPI**](https://github.com/VoidX3D/NewSheetAPI) | Sheet API service | JavaScript |

</div>

</details>

<details>
<summary><b>📚 Anime & Media (4)</b></summary>
<br>

<div align="center">

| Project | Description | Stack |
|:--------|:------------|:------|
| [**miruro**](https://github.com/VoidX3D/miruro) | Anime streaming platform | TypeScript |
| [**myanime**](https://github.com/VoidX3D/myanime) | Personal anime collection manager | TypeScript |
| [**Anilist-DB**](https://github.com/VoidX3D/Anilist-DB) | AniList GraphQL database integration | HTML, GraphQL |
| [**void-archive**](https://github.com/VoidX3D/void-archive) | Archive of Void projects | TypeScript |

</div>

</details>

<details>
<summary><b>🎓 School, Science & Experiments (4)</b></summary>
<br>

<div align="center">

| Project | Description | Stack |
|:--------|:------------|:------|
| [**sciencepresentation**](https://github.com/VoidX3D/sciencepresentation) | Science presentation web project | HTML, CSS, JS |
| [**science-study**](https://github.com/VoidX3D/science-study) | Science study tools & materials | HTML, CSS, JS |
| [**football-card-pack-**](https://github.com/VoidX3D/football-card-pack-) | Football card collection app | JavaScript |
| [**WebWebWeb**](https://github.com/VoidX3D/WebWebWeb) | Web experiment project | JavaScript |

</div>

</details>

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%">

---

<!-- ============================================ -->
<!--          CONTRIBUTION ACTIVITY               -->
<!-- ============================================ -->
<div align="center">

# 🐍 Contribution Activity

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

</div>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/voidx3d/voidx3d/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/voidx3d/voidx3d/output/github-contribution-grid-snake.svg">
  <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/voidx3d/voidx3d/output/github-contribution-grid-snake.svg">
</picture>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=voidx3d&bg_color=0d1117&color=00d9ff&line=00d9ff&point=ffffff&area=true&hide_border=true&custom_title=VoidX3D's%20Contribution%20Graph%202026&radius=10&theme=tokyo-night" alt="Activity Graph"/>
</div>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%">

---

<!-- ============================================ -->
<!--          DEVELOPER PHILOSOPHY                 -->
<!-- ============================================ -->
<div align="center">

# 💭 Developer Philosophy

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

</div>

```python
#!/usr/bin/env python3
"""
VoidX3D's Development Philosophy
================================
A comprehensive guide to my approach in software development
"""

from typing import Dict, List
from dataclasses import dataclass
from enum import Enum


class Priority(Enum):
    CRITICAL = 1
    HIGH = 2
    MEDIUM = 3
    LOW = 4


@dataclass
class Principle:
    name: str
    description: str
    priority: Priority
    examples: List[str]


class DeveloperPhilosophy:
    """Core principles that guide my development journey"""

    def __init__(self):
        self.principles = self._define_principles()
        self.daily_habits = self._define_habits()

    def _define_principles(self) -> List[Principle]:
        return [
            Principle("Clean Code Over Clever Code",
                      "Write code others can understand and maintain",
                      Priority.CRITICAL,
                      ["Descriptive variable names", "Comprehensive comments",
                       "Consistent style guides", "Small focused functions"]),
            Principle("Build to Learn, Not Just to Complete",
                      "Every project is a learning opportunity",
                      Priority.HIGH,
                      ["Experiment with new tech", "Document learnings",
                       "Share with community", "Reflect on improvements"]),
            Principle("Ship Early, Iterate Often",
                      "Done is better than perfect, but iterate toward excellence",
                      Priority.HIGH,
                      ["MVP first, features later", "Get feedback early",
                       "Continuous deployment", "Regular refactoring"]),
            Principle("Community Over Competition",
                      "Help others grow, and grow together",
                      Priority.HIGH,
                      ["Open source contributions", "Answer questions",
                       "Mentor juniors", "Share knowledge"]),
            Principle("Performance Matters, But Not Always First",
                      "Optimize where it counts, prioritize by impact",
                      Priority.MEDIUM,
                      ["Profile before optimizing", "Focus on bottlenecks",
                       "Consider UX", "Balance speed with maintainability"]),
        ]

    def _define_habits(self) -> Dict[str, List[str]]:
        return {
            "Morning": ["☕ Coffee + code review", "📧 GitHub notifications",
                        "📝 Plan today's tasks", "🎯 Set clear goals"],
            "Development": ["💻 Write clean code", "🧪 Test as you go",
                            "🔄 Commit frequently", "🤔 Ask when stuck"],
            "Learning": ["📚 Read technical articles", "🏗️ Build experimental projects",
                         "💡 Try new frameworks", "🎥 Watch tutorials"],
            "Evening": ["📊 Review progress", "📝 Document learnings",
                        "🎮 Relax with anime/games", "🔄 Plan tomorrow"],
        }

    def get_motivation(self) -> str:
        return """
        🗡️ Just like Ichigo's journey in Bleach:

        • Start as a beginner, grow through challenges
        • Each bug is a Hollow to defeat
        • Every project is a new Bankai to master
        • Protect what matters: clean code, users, community
        • Never give up, even when it seems impossible

        "I'm not Superman, so I can't say anything big like
        'I'll protect everyone on Earth!' I'm just a Soul Reaper
        who happens to be passing through. But if you get in my way...
        you're not going to live through this."

        Replace 'Soul Reaper' with 'Developer' — that's my coding motto! ⚔️
        """


philosophy = DeveloperPhilosophy()
print(philosophy.get_motivation())

# REMEMBER ALWAYS:
# ╔══════════════════════════════════════════════╗
# ║ "Code is read more often than it is written."║
# ║ "Make it work, make it right, make it fast." ║
# ║ "The best code is no code at all."           ║
# ║ "Programming is thinking, not typing."       ║
# ║ "Build things that matter.                   ║
# ║  Ship things that work.                      ║
# ║  Help people who need it.                    ║
# ║  Never stop learning."                       ║
# ╚══════════════════════════════════════════════╝
```

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%">

---

<!-- ============================================ -->
<!--          RANDOM DEV QUOTE                    -->
<!-- ============================================ -->
<div align="center">

# 💬 Random Dev Quote

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

</div>

<div align="center">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight&border=true" alt="Random Dev Quote"/>
</div>

<details>
<summary><b>📜 Click for some of my favorite quotes</b></summary>
<br>

<div align="center">

```ascii
╔══════════════════════════════════════════════════════════════════╗
║                                                                  ║
║  "First, solve the problem. Then, write the code."               ║
║                                        - John Johnson            ║
║                                                                  ║
║  "The best error message is the one that never shows up."        ║
║                                        - Thomas Fuchs            ║
║                                                                  ║
║  "Code is like humor. When you have to explain it, it's bad."    ║
║                                        - Cory House              ║
║                                                                  ║
║  "Make it work, make it right, make it fast."                    ║
║                                        - Kent Beck               ║
║                                                                  ║
║  "Any fool can write code that a computer can understand.        ║
║   Good programmers write code that humans can understand."       ║
║                                        - Martin Fowler           ║
║                                                                  ║
║  "Code with passion, debug with patience, deploy with pride!"    ║
║                                        - VoidX3D                 ║
║                                                                  ║
╚══════════════════════════════════════════════════════════════════╝
```

</div>

</details>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%">

---

<!-- ============================================ -->
<!--          FUN FACTS                           -->
<!-- ============================================ -->
<div align="center">

# ⚡ Fun Facts & Random Stuff

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

</div>

<table align="center">
  <tr>
    <td width="50%" valign="top">

### 🎌 Anime & Inspiration

- **Favorite Anime:** Bleach ⚔️
- **Favorite Character:** Ichigo Kurosaki
- **Why Bleach?** Constant growth, never giving up, epic battles mirror the dev journey
- **Coding Playlist:** Bleach OSTs + Lo-fi beats 🎧

### ☕ Coding Fuel

- **Drink of Choice:** Coffee (lots of it!)
- **Favorite Snack:** Instant noodles at 2 AM
- **Energy Source:** Determination + curiosity
- **Debugging Companion:** Rubber duck (seriously works!)

### 🎮 Gaming & Hobbies

- **Favorite Games:** Story-driven RPGs
- **Game Dev Interest:** Building my own engine
- **Creative Outlets:** Drawing pixel art, making music
- **Relaxation:** Long walks, mountain views (Nepal perks!)

    </td>
    <td width="50%" valign="top">

### 🏔️ Life in Nepal

- **Location:** Beautiful Pokhara city
- **Views:** Himalayas from my window 🏔️
- **Community:** Growing tech scene
- **Time Zone:** UTC+5:45 (yes, that's a real timezone!)
- **Internet:** Sometimes struggles, but we make it work

### 📚 Learning Style

- **Method:** 70% building, 20% reading, 10% tutorials
- **Best Time:** Late night coding sessions (night owl 🦉)
- **Learning From:** Errors, Stack Overflow, docs
- **Knowledge Sharing:** GitHub, Twitter threads, blogs

### 🎯 Random Dev Facts

- **First Language:** HTML/CSS (age 12)
- **First Real Project:** A calculator (we all start somewhere!)
- **Biggest Bug Hunt:** 6 hours — missing semicolon
- **Code Editor:** VS Code (50+ extensions)
- **Theme:** Tokyo Night — dark mode only! 💀
- **Commits:** Usually at odd hours (night owl confirmed 🦉)

    </td>
  </tr>
</table>

<div align="center">

### 🎨 Development Environment

```bash
╔══════════════════════════════════════════╗
║  💻 Hardware                              ║
║  • Laptop: Mid-range but gets job done    ║
║  • Keyboard: Mechanical (clicky clicks!)  ║
║  • Monitor: 1080p (dreaming of 4K)       ║
║                                           ║
║  🛠️ Software Stack                        ║
║  • OS: Windows 11 / Ubuntu dual boot      ║
║  • Terminal: Oh My Zsh + powerlevel10k    ║
║  • Editor: VS Code (Tokyo Night theme)    ║
║  • Browser: Chrome DevTools expert        ║
║  • Git: CLI only (I'm not a monster)      ║
║                                           ║
║  🎧 Coding Atmosphere                     ║
║  • Music: Lo-fi hip hop + Anime OSTs      ║
║  • Lighting: RGB everything 🌈            ║
║  • Drinks: Coffee machine always on       ║
║  • Time: 10 PM - 3 AM (peak hours) 🦉     ║
║  • Vibe: Dark mode, dim lights, focused   ║
╚══════════════════════════════════════════╝
```

</div>

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%">

---

<!-- ============================================ -->
<!--          CONNECT                             -->
<!-- ============================================ -->
<div align="center">

# 🌐 Connect With Me

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

I'm always open to collaboration, tech discussions, and new opportunities. Let's build something amazing together!

<br><br>

<a href="https://github.com/VoidX3D">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</a>
<a href="https://x.com/VortexVoidX3D?s=09">
  <img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="X"/>
</a>
<a href="https://www.instagram.com/sincerebhattarai/">
  <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram"/>
</a>
<a href="mailto:playzspreston2@gmail.com">
  <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"/>
</a>
<a href="https://voidx3d.netlify.app">
  <img src="https://img.shields.io/badge/Portfolio-00C7B7?style=for-the-badge&logo=netlify&logoColor=white" alt="Portfolio"/>
</a>
<a href="https://www.buymeacoffee.com/voidx3d">
  <img src="https://img.shields.io/badge/Buy_Me_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me A Coffee"/>
</a>

<br><br>

### 💬 Open For

🎁 Collaboration • 🎄 Open Source • ⛄ Freelance • 🎅 Mentorship • ❄️ Tech Discussions • 🎊 Project Ideas • 💡 Code Reviews

### 📍 Response Time

| Platform | Response Time |
|:---------|:-------------|
| 📧 Email | Within 24-48 hours |
| 🐦 X (Twitter) | Usually within hours |
| 💬 GitHub Issues | Best for technical questions |
| 📱 Instagram | Casual conversations |

</div>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%">

---

<!-- ============================================ -->
<!--          SUPPORT                             -->
<!-- ============================================ -->
<div align="center">

# 🤝 Support My Work

<img src="https://user-images.githubusercontent.com/74038190/213844263-a8897a51-32f4-4b3b-b5c2-e1528b89f6f3.png" width="50" />

If you like my projects and want to support my journey, here are some ways:

<br>

<a href="https://www.buymeacoffee.com/voidx3d">
  <img src="https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me A Coffee"/>
</a>
<a href="https://ko-fi.com/voidx3d">
  <img src="https://img.shields.io/badge/Ko--fi-FF5E5B?style=for-the-badge&logo=ko-fi&logoColor=white" alt="Ko-fi"/>
</a>
<a href="https://github.com/sponsors/VoidX3D">
  <img src="https://img.shields.io/badge/Sponsor-EA4AAA?style=for-the-badge&logo=github-sponsors&logoColor=white" alt="Sponsor"/>
</a>

<br><br>

<table>
  <tr>
    <td align="center" width="25%">
      <h4>⭐ Star Repositories</h4>
      <p>Give a star to repos you find useful</p>
    </td>
    <td align="center" width="25%">
      <h4>🔔 Follow Me</h4>
      <p>Stay updated with my projects</p>
    </td>
    <td align="center" width="25%">
      <h4>🤝 Collaborate</h4>
      <p>Work together on projects</p>
    </td>
    <td align="center" width="25%">
      <h4>🐛 Report Bugs</h4>
      <p>Help improve code quality</p>
    </td>
  </tr>
  <tr>
    <td align="center" width="25%">
      <h4>💡 Share Ideas</h4>
      <p>Suggest new features</p>
    </td>
    <td align="center" width="25%">
      <h4>📢 Spread Word</h4>
      <p>Share with your network</p>
    </td>
    <td align="center" width="25%">
      <h4>📝 Write Blogs</h4>
      <p>Write about my projects</p>
    </td>
    <td align="center" width="25%">
      <h4>🎁 Donate</h4>
      <p>Support via coffee/sponsor</p>
    </td>
  </tr>
</table>

</div>

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%">

---

<!-- ============================================ -->
<!--          EPIC ANIMATED FOOTER                -->
<!-- ============================================ -->
<div align="center">

<svg width="100%" height="220" viewBox="0 0 1000 220" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="footerGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00D9FF;stop-opacity:0.25" />
      <stop offset="50%" style="stop-color:#8A2BE2;stop-opacity:0.25" />
      <stop offset="100%" style="stop-color:#FF6B6B;stop-opacity:0.25" />
    </linearGradient>
    <linearGradient id="footerGrad2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#FF6B6B;stop-opacity:0.15" />
      <stop offset="50%" style="stop-color:#00D9FF;stop-opacity:0.15" />
      <stop offset="100%" style="stop-color:#8A2BE2;stop-opacity:0.15" />
    </linearGradient>
  </defs>

  <!-- Animated wave deep -->
  <path fill="url(#footerGrad)">
    <animate attributeName="d" dur="12s" repeatCount="indefinite"
      values="M0,120 Q250,70 500,120 T1000,120 L1000,220 L0,220 Z;
              M0,120 Q250,170 500,120 T1000,120 L1000,220 L0,220 Z;
              M0,120 Q250,70 500,120 T1000,120 L1000,220 L0,220 Z"/>
  </path>

  <!-- Animated wave shallow -->
  <path fill="url(#footerGrad2)">
    <animate attributeName="d" dur="9s" repeatCount="indefinite"
      values="M0,150 Q200,120 400,150 T800,150 T1000,140 L1000,220 L0,220 Z;
              M0,150 Q200,170 400,150 T800,150 T1000,160 L1000,220 L0,220 Z;
              M0,150 Q200,120 400,150 T800,150 T1000,140 L1000,220 L0,220 Z"/>
  </path>

  <!-- Footer text -->
  <text x="500" y="80" text-anchor="middle" fill="white" font-size="26" font-weight="bold" font-family="'Segoe UI', Arial">
    Thanks for visiting! 🌟
    <animate attributeName="opacity" values="1;0.7;1" dur="3s" repeatCount="indefinite"/>
  </text>

  <text x="500" y="115" text-anchor="middle" fill="#00D9FF" font-size="14" font-family="monospace">
    ⚡ Powered by passion, coffee, and determination
  </text>

  <text x="500" y="140" text-anchor="middle" fill="#8b949e" font-size="13" font-family="monospace">
    Made with ❤️ by VoidX3D  |  © 2024-2026  |  Pokhara, Nepal 🇳🇵
  </text>

  <text x="500" y="168" text-anchor="middle" fill="#484f58" font-size="12" font-family="monospace" letter-spacing="2">
    BUILDING  •  LEARNING  •  SHIPPING  •  NEVER  STOPPING  🚀
  </text>

  <!-- Small decorative dots -->
  <circle cx="480" y="190" r="2" fill="#00D9FF" opacity="0.4">
    <animate attributeName="opacity" values="0.4;0.1;0.4" dur="2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="500" cy="190" r="2" fill="#8A2BE2" opacity="0.4">
    <animate attributeName="opacity" values="0.4;0.1;0.4" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="520" cy="190" r="2" fill="#FF6B6B" opacity="0.4">
    <animate attributeName="opacity" values="0.4;0.1;0.4" dur="3s" repeatCount="indefinite"/>
  </circle>
</svg>

<img src="https://capsule-render.vercel.app/api?type=waving&height=120&color=gradient&customColorList=6,11,20&section=footer&text=Keep%20Coding!%20%E2%9A%94%EF%B8%8F&fontSize=28&fontColor=fff&animation=twinkling&fontAlignY=60"/>

<br>

<sub>
  ⚡ Built with Markdown + SVG Animations + Local Icons (57) + Pure Passion 💖<br>
  🎮 Currently coding at 2 AM with coffee, lo-fi beats, and zero bugs (we can dream) 🎧
</sub>

---

</div>
