```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>The Code Alchemist</title>
    <style>
      :root {
        --primary: #2b3137;
        --secondary: #444d56;
        --accent: #0366d6;
        --text: #c9d1d9;
        --highlight: #58a6ff;
        --card-bg: #161b22;
        --font-main: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica,
          Arial, sans-serif;
        --font-code: "SFMono-Regular", Consolas, "Liberation Mono", Menlo,
          monospace;
      }
      [data-color-mode="light"] {
        --primary: #f6f8fa;
        --secondary: #e1e4e8;
        --accent: #0366d6;
        --text: #24292e;
        --highlight: #0366d6;
        --card-bg: #ffffff;
      }
      body {
        font-family: var(--font-main);
        background-color: var(--primary);
        color: var(--text);
        line-height: 1.6;
        margin: 0;
        padding: 20px;
        max-width: 900px;
        margin: 0 auto;
        transition: background-color 0.3s ease, color 0.3s ease;
      }
      header {
        display: flex;
        align-items: center;
        margin-bottom: 30px;
        border-bottom: 1px solid var(--secondary);
        padding-bottom: 20px;
      }
      .avatar {
        width: 120px;
        height: 120px;
        border-radius: 50%;
        border: 4px solid var(--accent);
        margin-right: 30px;
        object-fit: cover;
      }
      h1 {
        color: var(--highlight);
        margin: 0;
        font-size: 2.2em;
      }
      .tagline {
        font-style: italic;
        color: var(--text);
        opacity: 0.8;
        margin: 5px 0 10px;
      }
      .social-links {
        display: flex;
        gap: 15px;
      }
      .social-links a {
        color: var(--highlight);
        text-decoration: none;
        transition: all 0.3s ease;
      }
      .social-links a:hover {
        text-decoration: underline;
        color: var(--accent);
      }
      section {
        margin-bottom: 30px;
        background: var(--card-bg);
        padding: 20px;
        border-radius: 6px;
        border: 1px solid var(--secondary);
        transition: background-color 0.3s ease, border-color 0.3s ease;
      }
      h2 {
        color: var(--highlight);
        margin-top: 0;
        border-bottom: 1px solid var(--secondary);
        padding-bottom: 10px;
      }
      .skills {
        display: flex;
        flex-wrap: wrap;
        gap: 10px;
      }
      .skill {
        background: var(--accent);
        color: white;
        padding: 5px 10px;
        border-radius: 20px;
        font-size: 0.9em;
      }
      .projects {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
        gap: 20px;
      }
      .project-card {
        background: var(--card-bg);
        border: 1px solid var(--secondary);
        border-radius: 6px;
        padding: 15px;
        transition: transform 0.3s ease, border-color 0.3s ease;
      }
      .project-card:hover {
        transform: translateY(-5px);
        border-color: var(--accent);
      }
      .project-title {
        color: var(--highlight);
        margin: 0 0 10px;
        font-size: 1.2em;
      }
      .project-desc {
        font-size: 0.9em;
        margin-bottom: 15px;
      }
      .project-tech {
        display: flex;
        flex-wrap: wrap;
        gap: 8px;
        font-size: 0.8em;
      }
      .project-tech span {
        background: rgba(3, 102, 214, 0.1);
        color: var(--highlight);
        padding: 3px 8px;
        border-radius: 20px;
      }
      footer {
        text-align: center;
        margin-top: 40px;
        padding-top: 20px;
        border-top: 1px solid var(--secondary);
        font-size: 0.9em;
        color: var(--text);
        opacity: 0.7;
      }
      .quote {
        font-style: italic;
        padding: 15px;
        background: rgba(3, 102, 214, 0.1);
        border-left: 3px solid var(--accent);
        margin: 20px 0;
      }
      .theme-toggle {
        position: fixed;
        top: 20px;
        right: 20px;
        background: var(--card-bg);
        border: 1px solid var(--secondary);
        border-radius: 50%;
        width: 40px;
        height: 40px;
        display: flex;
        align-items: center;
        justify-content: center;
        cursor: pointer;
        z-index: 100;
        transition: all 0.3s ease;
      }
      .theme-toggle:hover {
        border-color: var(--accent);
      }
      @media (max-width: 768px) {
        header {
          flex-direction: column;
          text-align: center;
        }
        .avatar {
          margin-right: 0;
          margin-bottom: 20px;
        }
        .social-links {
          justify-content: center;
        }
        .theme-toggle {
          top: 10px;
          right: 10px;
        }
      }
    </style>
  </head>
  <body>
    <div class="theme-toggle" id="themeToggle">
      <svg
        id="themeIcon"
        width="20"
        height="20"
        viewBox="0 0 24 24"
        fill="none"
        stroke="currentColor"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <!-- Default is moon icon for dark mode -->
        <path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
      </svg>
    </div>
    <header>
      <img
        src="https://avatars.githubusercontent.com/u/76515367?v=4"
        alt="Profile Picture"
        class="avatar"
      />
      <div>
        <h1>Geoffrey Owuor</h1>
        <p class="tagline">Turning caffeine into code since 2020</p>
        <div class="social-links">
          <a href="https://github.com/Geoffrey-Owuor" target="_blank">GitHub</a>
          <a href="https://www.linkedin.com/in/owuor-geoffrey22" target="_blank"
            >LinkedIn</a
          >
          <a href="https://x.com/OwuorOkinyi22" target="_blank">Twitter(X)</a>
          <a href="mailto:geoffreyowuor22@gmail.com">Email</a>
        </div>
      </div>
    </header>
    <section>
      <h2>👨‍💻 About Me</h2>
      <p>
        Software Engineer | Full-Stack Wizard | Problem Solver | Professional
        Debugger
      </p>
      <div class="quote">
        "I don't always write bugs, but when I do, they're in production."
      </div>
      <p>
        With a keyboard as my wand and Stack Overflow as my spellbook, I conjure
        digital solutions out of thin air. When I'm not wrestling with
        JavaScript frameworks or debating tabs vs spaces, I'm probably
        explaining to my family that "no, I can't fix your printer."
      </p>
      <p>
        I believe in writing code that's so clean even my future self won't
        curse my past self. My superpower? Turning complex problems into elegant
        solutions while maintaining a healthy relationship with my rubber duck.
      </p>
    </section>
    <section>
      <h2>🛠️ Tech Stack</h2>
      <p>
        Here's the arsenal of technologies I wield with varying degrees of
        competence:
      </p>
      <div class="skills">
        <span class="skill">JavaScript</span>
        <span class="skill">TypeScript</span>
        <span class="skill">React</span>
        <span class="skill">Node.js</span>
        <span class="skill">Python</span>
        <span class="skill">Java</span>
        <span class="skill">SQL</span>
        <span class="skill">NoSQL</span>
        <span class="skill">Git</span>
        <span class="skill">NextJS</span>
        <span class="skill">Linux</span>
        <span class="skill">Agile</span>
      </div>
    </section>
    <section>
      <h2>🚀 Current Projects</h2>
      <p>
        Here's what's currently keeping me up at night (besides my poor life
        choices and that one unresolved GitHub issue):
      </p>
      <div class="projects">
        <div class="project-card">
          <h3 class="project-title">Sass Inventory Software</h3>
          <p class="project-desc">
            From the name itself, an inventory web app, made with NextJS
          </p>
          <div class="project-tech">
            <span>NextJS</span>
            <span>MongoDB</span>
            <span>Prisma</span>
          </div>
        </div>
        <div class="project-card">
          <h3 class="project-title">Form Requisitions Automation</h3>
          <p class="project-desc">
            Automating new requisitions using google forms, google sheets, and
            google apps script. Unique right? , probably not.
          </p>
          <div class="project-tech">
            <span>G script</span>
            <span>Google Sheets</span>
            <span>Google Forms</span>
          </div>
        </div>
        <div class="project-card">
          <h3 class="project-title">Online Garbage Collection Software</h3>
          <p class="project-desc">
            Sounds crazy I know, but believe me, have you ever thought of
            ordering for garbage collection services the way you order your
            Uber?
          </p>
          <div class="project-tech">
            <span>JavaScript</span>
            <span>PHP</span>
            <span>HTML/CSS</span>
          </div>
        </div>
      </div>
    </section>
    <section>
      <h2>📈 GitHub Stats</h2>
      <div
        style="display: flex; justify-content: space-between; flex-wrap: wrap"
      >
        <img
          id="githubStats"
          src="https://github-readme-stats.vercel.app/api?username=Geoffrey-Owuor&show_icons=true&theme=dark"
          alt="GitHub Stats"
          style="max-width: 100%"
        />
        <img
          id="githubTopLangs"
          src="https://github-readme-stats.vercel.app/api/top-langs/?username=Geoffrey-Owuor&layout=compact&theme=dark"
          alt="Top Languages"
          style="max-width: 100%"
        />
      </div>
    </section>
    <footer>
      <p>Made with ❤️, ☕, and probably too much time in VSCode</p>
      <p>Last updated: <span id="last-updated"></span></p>
    </footer>
    <script>
      // Simple script to show last updated date
      document.getElementById("last-updated").textContent =
        new Date().toLocaleDateString("en-US", {
          year: "numeric",
          month: "long",
          day: "numeric",
        });
      let originalTitle = document.title;
      window.addEventListener("blur", () => {
        document.title = "👀 Where are you going?";
      });
      window.addEventListener("focus", () => {
        document.title = originalTitle;
      });
      // Theme toggle functionality
      const themeToggle = document.getElementById("themeToggle");
      const themeIcon = document.getElementById("themeIcon");
      const githubStats = document.getElementById("githubStats");
      const githubTopLangs = document.getElementById("githubTopLangs");
      // Check for saved theme preference or use system preference
      const savedTheme = localStorage.getItem("theme");
      const systemPrefersDark = window.matchMedia(
        "(prefers-color-scheme: dark)"
      ).matches;
      let currentTheme = savedTheme || (systemPrefersDark ? "dark" : "light");
      setTheme(currentTheme);
      // Toggle theme on button click
      themeToggle.addEventListener("click", () => {
        currentTheme = currentTheme === "dark" ? "light" : "dark";
        setTheme(currentTheme);
        localStorage.setItem("theme", currentTheme);
      });
      function setTheme(theme) {
        document.documentElement.setAttribute("data-color-mode", theme);
        // Update GitHub stats images based on theme
        const themeParam = theme === "dark" ? "dark" : "default";
        githubStats.src = `https://github-readme-stats.vercel.app/api?username=Geoffrey-Owuor&show_icons=true&theme=${themeParam}`;
        githubTopLangs.src = `https://github-readme-stats.vercel.app/api/top-langs/?username=Geoffrey-Owuor&layout=compact&theme=${themeParam}`;
        // Update icon
        if (theme === "dark") {
          themeIcon.innerHTML =
            '<path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>';
        } else {
          themeIcon.innerHTML =
            '<circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line>';
        }
      }
      // Sync with GitHub's theme if embedded
      if (window.parent !== window) {
        const observer = new MutationObserver(() => {
          const githubTheme =
            document.documentElement.getAttribute("data-color-mode");
          if (githubTheme && githubTheme !== currentTheme) {
            currentTheme = githubTheme;
            setTheme(currentTheme);
            localStorage.setItem("theme", currentTheme);
          }
        });
        observer.observe(document.documentElement, {
          attributes: true,
          attributeFilter: ["data-color-mode"],
        });
      }
    </script>
  </body>
</html>
```

### 👋 Hello World!

I'm Geoffrey Owuor, a software engineer who believes in making technology work for humans (most of the time).

🔭 **Currently working on:** Saas Inventory Software
🌱 **Currently learning:** How to explain blockchain to my mother
👯 **Looking to collaborate on:** Projects that make developers' lives easier  
💬 **Ask me about:** Why semicolons are optional but your love life isn't  
📫 **How to reach me:** carrier pigeon preferred, but email works too  
⚡ **Fun fact:** I once fixed a bug by turning it off and on again
