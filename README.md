<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Geoffrey | Software Engineer</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Inter', sans-serif;
      background: linear-gradient(135deg, #0f172a, #1e293b);
      color: #e2e8f0;
      padding: 2rem;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .container {
      max-width: 800px;
      background: #1e293b;
      padding: 2rem;
      border-radius: 1rem;
      box-shadow: 0 0 30px rgba(0,0,0,0.3);
    }
    h1 {
      font-size: 2.5rem;
      color: #38bdf8;
      text-align: center;
    }
    p {
      margin-top: 1rem;
      line-height: 1.6;
      font-size: 1.1rem;
    }
    .highlight {
      color: #22d3ee;
      font-weight: 600;
    }
    ul {
      margin-top: 1rem;
      padding-left: 1.5rem;
    }
    li {
      margin-bottom: 0.6rem;
    }
    .project-title {
      color: #facc15;
      font-weight: 600;
    }
    .fun-fact {
      font-style: italic;
      color: #a5f3fc;
      margin-top: 2rem;
    }
    .fade-in {
      opacity: 0;
      transform: translateY(30px);
      transition: all 0.6s ease-out;
    }
    .fade-in.visible {
      opacity: 1;
      transform: translateY(0);
    }
  </style>
</head>
<body>
  <div class="container fade-in" id="main">
    <h1>Hi, I’m Geoffrey 👨🏾‍💻</h1>
    <p>
      A <span class="highlight">Software Engineer</span> with a passion for clean code, elegant UI, and sneaking humor into comments where no one dares to look.
      I recently graduated <span class="highlight">First Class Honors 🎓</span> in Computer Science and have professional experience in
      <span class="highlight">full-stack development</span>, <span class="highlight">technical support</span>, and <span class="highlight">server maintenance</span>. I’ve also interned at
      <strong>Kenya Tea Development Agency (KTDA)</strong>—yes, I bring the flavor 🍵.
    </p>

    <p>
      You’ll usually find me coding in <span class="highlight">PHP</span>, <span class="highlight">JavaScript</span>, or <span class="highlight">Python</span>,
      styling with <span class="highlight">CSS (the respectful kind)</span>, and building front-ends with <span class="highlight">React</span>. 
      I'm currently learning <span class="highlight">Figma</span> to make sure my UIs not only work great, but look good enough to screenshot.
    </p>

    <h2 style="margin-top:2rem; color:#38bdf8;">🔧 Projects I'm Currently Cooking</h2>
    <ul>
      <li>
        <span class="project-title">KTDA IT Toolkit</span>: A sleek web-based dashboard that simplifies technical support operations — from LAN troubleshooting to biometric systems maintenance.
      </li>
      <li>
        <span class="project-title">Mini Data Pipeline</span>: A side project built with Python that mimics ETL processes and prepares me for my dream job as a Data Engineer (MixRank, I’m looking at you 👀).
      </li>
      <li>
        <span class="project-title">React Portfolio Revamp</span>: Rebuilding my personal site with Tailwind, React, and a sprinkle of Framer Motion — because every click should feel like magic ✨.
      </li>
    </ul>

    <p class="fun-fact">Fun Fact: I once fixed a printer jam, rewired a network, and installed a SQL patch — all before lunch. They called me "the Swiss Army Dev."</p>
  </div>

  <script>
    // Smooth fade-in animation
    window.addEventListener('DOMContentLoaded', () => {
      const fadeIn = document.querySelector('.fade-in');
      setTimeout(() => {
        fadeIn.classList.add('visible');
      }, 300);
    });
  </script>
</body>
</html>
