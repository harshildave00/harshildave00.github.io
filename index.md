---
layout: default
title: Home
---

<nav class="main-nav">
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#experience">Experience</a>
  <a href="#projects">Projects</a>
  <a href="#skills">Skills</a>
</nav>

<section id="home" class="hero">
  <div class="hero-content">
    <img src="assets/images/profile.jpg" alt="Harshil Dave" class="profile-img">
    <h1>Hi, I’m Harshil Dave</h1>
    <p class="hero-sub">Data Science Student | Software Developer | AI Enthusiast</p>
    <p><a href="assets/HarshilDave_Resume.pdf" class="btn">Download Resume</a></p>
    <p class="contact-info">Chapel Hill, NC | <a href="mailto:hmdave@unc.edu">hmdave@unc.edu</a> | +1-919-656-1121</p>
  </div>
</section>

<section id="about" class="fade-in">
  <h2>About Me</h2>
  <p>
    I’m a Data Science student at UNC Chapel Hill, passionate about software development, AI, and data analytics.
    My experience in internships, research, and leadership equips me with problem-solving skills, teamwork,
    and the ability to deliver impactful projects.
  </p>
</section>

<section id="experience" class="fade-in">
  <h2>Experience</h2>
  <div class="cards-container">
    <div class="item">
      <strong>Data Science Intern – Sports Media</strong>
      <span class="muted">June 2025 – Jan 2026</span>
      <p>Assisted with market research, trend analysis, social media campaigns, and digital marketing strategies.</p>
    </div>
    <div class="item">
      <strong>Data Analyst – UNC Women’s Tennis</strong>
      <span class="muted">Oct 2025 – Present</span>
      <p>Tracked performance statistics, tagged match film, and built dashboards for coaching staff.</p>
    </div>
    <div class="item">
      <strong>Lead Instructional Assistant – UNC Charlotte</strong>
      <span class="muted">Aug 2023 – Jun 2024</span>
      <p>Delivered interactive lessons, mentored students, and improved grading efficiency by 40%.</p>
    </div>
  </div>
</section>

<section id="leadership" class="fade-in">
  <h2>Leadership</h2>
  <div class="cards-container">
    <div class="item">
      <strong>Chairman & Business Lead – InspireNC</strong>
      <span class="muted">Oct 2020 – Aug 2023</span>
      <p>Secured $15,000+ in grants, organized 10+ community events, and promoted STEAM education to 300+ students.</p>
    </div>
  </div>
</section>

<section id="projects" class="fade-in">
  <h2>Projects</h2>
  <div class="cards-container">
    <div class="item">
      <strong>Interactive Dashboard<strong>
      <p>Built an interactive dashboard displaying reviews for British Airways.<a href="https://public.tableau.com/views/TableauProject1_17525916320900/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link">Tableau</a></p>
    </div>
    <div class="item">
      <strong>Data Analysis Tool</strong>
      <p>Python tool to analyze & visualize large datasets; improved processing speed by 30%.</p>
    </div>
    <div class="item">
      <strong>Project Portfolio</strong>
      <p><a href="https://opal.ils.unc.edu/~hmdave/">Live portfolio of academic and personal projects</a></p>
    </div>
  </div>
</section>

<section id="skills" class="fade-in">
  <h2>Skills & Certifications</h2>
  <ul class="skills-list">
    <li>Python | Java | HTML | R | SAS | SQL</li>
    <li>Pivot Tables, Charts, MS SQL Server</li>
    <li>MTA Python | Microsoft Office Specialist | Adobe Certified Professional (Photoshop, Illustrator, Graphic Design)</li>
  </ul>
</section>

<script>
const sections = document.querySelectorAll("section");
const navLinks = document.querySelectorAll(".main-nav a");

window.addEventListener("scroll", () => {
  let current = "";
  sections.forEach(section => {
    const sectionTop = section.offsetTop - 100;
    if (scrollY >= sectionTop) current = section.getAttribute("id");
  });
  navLinks.forEach(link => {
    link.classList.remove("active");
    if (link.getAttribute("href") === "#" + current) link.classList.add("active");
  });
});
</script>
