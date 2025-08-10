<!-- Liquid Glass — Animated Floating Panels README -->
<p align="center">
  <!-- Animated Liquid Glass SVG (SMIL-based) -->
  <svg width="880" height="260" viewBox="0 0 880 260" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Liquid glass animated header">
    <defs>
      <!-- soft glass gradient -->
      <linearGradient id="g1" x1="0" x2="1" y1="0" y2="1">
        <stop offset="0" stop-color="#00f7ff" stop-opacity="0.18"/>
        <stop offset="1" stop-color="#7c4dff" stop-opacity="0.12"/>
      </linearGradient>

      <linearGradient id="g2" x1="0" x2="1" y1="0" y2="1">
        <stop offset="0" stop-color="#00f7ff" stop-opacity="0.14"/>
        <stop offset="1" stop-color="#ff7ad1" stop-opacity="0.10"/>
      </linearGradient>

      <!-- subtle highlight -->
      <linearGradient id="shine" x1="0" x2="0" y1="0" y2="1">
        <stop offset="0" stop-color="#ffffff" stop-opacity="0.35"/>
        <stop offset="1" stop-color="#ffffff" stop-opacity="0.02"/>
      </linearGradient>

      <!-- rounded mask so inner strokes look smooth -->
      <mask id="softmask">
        <rect x="0" y="0" width="880" height="260" fill="white" rx="20" ry="20"/>
      </mask>
    </defs>

    <!-- background vignette -->
    <rect width="100%" height="100%" fill="#05060a" rx="14" ry="14"/>

    <!-- floating glass panel group -->
    <!-- Panel 1 -->
    <g transform="translate(90,30)">
      <rect x="0" y="0" rx="16" ry="16" width="240" height="160"
        fill="url(#g1)"
        stroke="rgba(255,255,255,0.08)" stroke-width="1.2"/>
      <!-- highlight -->
      <rect x="6" y="6" rx="12" ry="12" width="228" height="40" fill="url(#shine)" opacity="0.5"/>

      <!-- subtle inner content: title + bullets as rectangles -->
      <rect x="18" y="62" width="180" height="14" rx="6" fill="rgba(255,255,255,0.06)"/>
      <rect x="18" y="86" width="140" height="10" rx="5" fill="rgba(255,255,255,0.04)"/>
      <rect x="18" y="102" width="160" height="10" rx="5" fill="rgba(255,255,255,0.04)"/>

      <!-- floating animation (vertical) -->
      <animateTransform attributeName="transform"
        type="translate"
        from="90 30" to="90 36"
        dur="3.8s"
        begin="0s"
        repeatCount="indefinite"
        additive="sum"
        fill="freeze"/>
    </g>

    <!-- Panel 2 (center, largest) -->
    <g transform="translate(320,10)">
      <rect x="0" y="0" rx="18" ry="18" width="380" height="200"
        fill="url(#g2)"
        stroke="rgba(255,255,255,0.09)" stroke-width="1.4"/>
      <rect x="10" y="10" rx="14" ry="14" width="360" height="50" fill="url(#shine)" opacity="0.45"/>

      <!-- fake cards inside -->
      <rect x="24" y="74" width="120" height="16" rx="8" fill="rgba(255,255,255,0.06)"/>
      <rect x="24" y="96" width="260" height="12" rx="6" fill="rgba(255,255,255,0.04)"/>
      <rect x="24" y="112" width="200" height="12" rx="6" fill="rgba(255,255,255,0.04)"/>
      <rect x="24" y="132" width="140" height="12" rx="6" fill="rgba(255,255,255,0.04)"/>

      <!-- small floating accent circle -->
      <circle cx="320" cy="36" r="8" fill="#00f7ff" opacity="0.95"/>

      <!-- subtle rotation + vertical float for a more organic motion -->
      <animateTransform attributeName="transform"
        type="translate"
        from="320 10" to="320 16"
        dur="4.4s"
        begin="0s"
        repeatCount="indefinite"
        additive="sum"
        fill="freeze"/>
      <animateTransform attributeName="transform"
        type="rotate"
        from="0 190 100" to="-0.8 190 100"
        dur="6s"
        begin="0s"
        repeatCount="indefinite"
        additive="sum"
        fill="freeze"/>
    </g>

    <!-- Panel 3 (right) -->
    <g transform="translate(730,50)">
      <rect x="-160" y="0" rx="14" ry="14" width="200" height="120"
        fill="url(#g1)"
        stroke="rgba(255,255,255,0.08)" stroke-width="1.1"/>
      <rect x="-152" y="8" rx="10" ry="10" width="184" height="34" fill="url(#shine)" opacity="0.45"/>
      <rect x="-140" y="56" width="140" height="12" rx="6" fill="rgba(255,255,255,0.05)"/>
      <rect x="-140" y="74" width="110" height="12" rx="6" fill="rgba(255,255,255,0.04)"/>

      <animateTransform attributeName="transform"
        type="translate"
        from="730 50" to="730 44"
        dur="3.2s"
        begin="0s"
        repeatCount="indefinite"
        additive="sum"
        fill="freeze"/>
      <animateTransform attributeName="transform"
        type="rotate"
        from="0 620 60" to="0.6 620 60"
        dur="5.2s"
        begin="0s"
        repeatCount="indefinite"
        additive="sum"
        fill="freeze"/>
    </g>

    <!-- center title text -->
    <g transform="translate(440,210)" text-anchor="middle" fill="#cfefff" font-family="Inter, Arial, sans-serif">
      <text x="0" y="-2" font-size="20" font-weight="700">Hey — I build cool things ✨</text>
      <text x="0" y="18" font-size="12" fill="#9fdcff">Liquid glass UI · AI · Web · Open Source</text>
    </g>
  </svg>
</p>

<!-- Main glass container -->
<div style="
  background: rgba(255,255,255,0.04);
  border-radius: 16px;
  padding: 20px;
  max-width: 960px;
  margin: 18px auto;
  border: 1px solid rgba(255,255,255,0.06);
  backdrop-filter: blur(6px);
  -webkit-backdrop-filter: blur(6px);
  box-shadow: 0 6px 28px rgba(2,6,23,0.55);
">

<h1 align="center" style="color:#e6fbff">Hi, I'm <span style="color:#00f7ff">YOUR NAME</span> 👋</h1>

<p align="center" style="color:#bfeeff; max-width:820px; margin:auto;">
A dev who loves futuristic UI, clean code, and shipping practical AI. I combine glassmorphism, micro-interactions, and strong engineering to make delightful products.
</p>

## 🔭 Featured Projects
- **Project Alpha** — An AI-powered assistant with RAG + agents.  
- **Liquid UI Kit** — Reusable components & CSS utilities for glassy designs.  
- **Lie Detector AI** — Fun React/Next.js experiment with audio UX.

## 🛠 Tech & Tools
<p>
  <img src="https://skillicons.dev/icons?i=react,nextjs,js,ts,python,tailwind,azure,git" alt="tech icons" />
</p>

## 📈 GitHub Stats
<p>
  <img src="https://github-readme-stats.vercel.app/api?username=YOURUSERNAME&show_icons=true&theme=transparent&hide_border=true&title_color=00f7ff&icon_color=00f7ff&text_color=bfeeff" alt="github stats" />
</p>

## 📫 Connect
<p>
  <a href="https://linkedin.com/in/YOURUSERNAME" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-00f7ff?style=for-the-badge&logo=linkedin&logoColor=black" alt="LinkedIn" /></a>
  <a href="mailto:you@example.com"><img src="https://img.shields.io/badge/Email-00f7ff?style=for-the-badge&logo=gmail&logoColor=black" alt="Email" /></a>
  <a href="https://twitter.com/YOURUSERNAME" target="_blank"><img src="https://img.shields.io/badge/X-00f7ff?style=for-the-badge&logo=x&logoColor=black" alt="X" /></a>
</p>

</div>

<p align="center" style="color:#9fcff7; margin-top:10px;">
  💠 Crafted with a liquid glass aesthetic • tweak colors & content below
</p>
