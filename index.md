---
layout: default
title: Home
---

<!-- Navigation -->
<nav class="main-nav">
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#experience">Experience</a>
  <a href="#projects">Projects</a>
  <a href="#skills">Skills</a>
</nav>

<!-- Home / Hero Section -->
<section id="home" class="hero">
  <img src="assets/images/profile.jpg" alt="Harshil Dave" class="profile-img">
  <h1>Hi, I’m Harshil Dave</h1>
  <p class="hero-sub">Data Science Student | Software Development | AI Enthusiast</p>
  <p><a href="assets/HarshilDave_Resume.pdf" class="btn">Download Resume</a></p>
  <p>Chapel Hill, NC | <a href="mailto:hmdave@unc.edu">hmdave@unc.edu</a> | +1-919-656-1121</p>
</section>

<!-- About Section -->
<section id="about">
  <h2>About Me</h2>
  <p>
    I’m a Data Science student at the University of North Carolina at Chapel Hill, passionate about software development,
    AI, and data analysis. My experiences in research, internships, and leadership have equipped me with problem-solving skills,
    teamwork, and the ability to deliver impactful projects.
  </p>
</section>

<!-- Experience Section -->
<section id="experience">
  <h2>Experience</h2>

  <div class="item">
    <strong>Data Science Intern – Sports Media, Severance, CO</strong><br>
    <span class="muted">June 2025 – January 2026</span>
    <p>
      Assisted with market research, trend analysis, and data collection. Supported social media campaigns
      and collaborated with teams to improve campaign performance.
    </p>
  </div>

  <div class="item">
    <strong>Data Analyst – UNC Women’s Tennis</strong><br>
    <span class="muted">October 2025 – Present</span>
    <p>
      Tracked performance statistics, rewatched match film with metadata tagging, and built dashboards
      for coaching staff to optimize performance.
    </p>
  </div>

  <div class="item">
    <strong>Lead Instructional Assistant – UNC Charlotte</strong><br>
    <span class="muted">August 2023 – June 2024</span>
    <p>
      Delivered 75+ interactive lesson plans, mentored 50+ students, and improved grading efficiency by 40%
      managing a team of 5 TAs.
    </p>
  </div>
</section>

<!-- Leadership Section -->
<section id="leadership">
  <h2>Leadership</h2>

  <div class="item">
    <strong>Chairman & Business Lead – InspireNC, Raleigh NC</strong><br>
    <span class="muted">October 2020 – August 2023</span>
    <p>
      Secured $15,000+ in grants, organized 10+ STEAM events for 300+ students, and promoted robotics initiatives.
    </p>
  </div>
</section>

<!-- Projects Section -->
<section id="projects">
  <h2>Projects</h2>

  <div class="item">
    <strong>Portfolio Website</strong>
    <p>
      Personal portfolio website built with Jekyll and GitHub Pages. 
      <a href="https://github.com/harshildave00">GitHub</a>
    </p>
  </div>

  <div class="item">
    <strong>Data Analysis Tool</strong>
    <p>
      Python tool for analyzing and visualizing large datasets, improving processing speed by 30%.
    </p>
  </div>

  <div class="item">
    <strong>Project Portfolio</strong>
    <p>
      <a href="https://opal.ils.unc.edu/~hmdave/">Live portfolio of academic and personal projects</a>
    </p>
  </div>
</section>

<!-- Skills Section -->
<section id="skills">
  <h2>Skills & Certifications</h2>
  <ul>
    <li>Programming: Python | Java | HTML | R | SAS | SQL</li>
    <li>Data Tools: Pivot Tables, Charts, MS SQL Server</li>
    <li>Certifications: MTA Python | Microsoft Office Specialist | Adobe Certified Professional (Photoshop, Illustrator, Graphic Design)</li>
  </ul>
</section>

<!-- Active tab script -->
<script>
const sections = document.querySelectorAll("section");
const navLinks = document.querySelectorAll(".main-nav a");

window.addEventListener("scroll", () => {
  let current = "";
  sections.forEach(section => {
    const sectionTop = section.offsetTop - 80;
    if (scrollY >= sectionTop) current = section.getAttribute("id");
  });

  navLinks.forEach(link => {
    link.classList.remove("active");
    if (link.getAttribute("href") === "#" + current) {
      link.classList.add("active");
    }
  });
});
</script>
