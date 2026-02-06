---
layout: default
title: Home
---

<!-- Navigation -->
<nav class="main-nav">
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#experience">Experience</a>
  <a href="#leadership">Leadership</a>
  <a href="#projects">Projects</a>
  <a href="#skills">Skills</a>
</nav>

<!-- Hero / Home Section -->
<section id="home" class="hero fade-in">
  <div class="hero-content">
    <h1>Hi, I’m Harshil Dave</h1>
    <p class="hero-sub">Data Science Student | Software Developer | AI Enthusiast</p>
    <p><a href="assets/HarshilDave_Resume.pdf" class="btn">Download Resume</a></p>
    <p class="contact-info">Chapel Hill, NC | <a href="mailto:hmdave@unc.edu">hmdave@unc.edu</a> | +1-919-656-1121</p>
  </div>
</section>

<!-- About Section -->
<section id="about" class="fade-in">
  <h2>About Me</h2>
  <p>
    I’m a Data Science student at UNC Chapel Hill, passionate about software development, AI, and data analytics.
    My experiences in internships, research, and leadership equip me with problem-solving skills, teamwork,
    and the ability to deliver impactful projects.
  </p>
</section>

<!-- Experience Section -->
<section id="experience" class="fade-in">
  <h2>Experience</h2>
  <div class="cards-container">
    <div class="item fade-card">
      <strong>Data Science Intern – Sports Media, Severance, CO</strong>
      <span class="muted">June 2025 – Jan 2026</span>
      <p>Assisted with market research, trend analysis, social media campaigns, and digital marketing strategies.</p>
    </div>
    <div class="item fade-card">
      <strong>Data Analyst – UNC Women’s Tennis</strong>
      <span class="muted">Oct 2025 – Present</span>
      <p>Tracked performance statistics, tagged match film, and built dashboards for coaching staff.</p>
    </div>
    <div class="item fade-card">
      <strong>Lead Instructional Assistant – UNC Charlotte</strong>
      <span class="muted">Aug 2023 – Jun 2024</span>
      <p>Delivered interactive lessons, mentored 50+ students, and improved grading efficiency by 40%.</p>
    </div>
  </div>
</section>

<!-- Leadership Section -->
<section id="leadership" class="fade-in">
  <h2>Leadership</h2>
  <div class="cards-container">
    <div class="item fade-card">
      <strong>Chairman & Business Lead – InspireNC, Raleigh NC</strong>
      <span class="muted">Oct 2020 – Aug 2023</span>
      <p>Secured $15,000+ in grants, organized 10+ community events, and promoted STEAM education to 300+ students.</p>
    </div>
  </div>
</section>

<!-- Projects Section -->
<section id="projects" class="fade-in">
  <h2>Projects</h2>
  <div class="cards-container">
    <div class="item fade-card">
      <strong>Interactive Dashboard</strong>
      <p>Build an interactive dashboard that displays reviews for British airways. <a href="https://public.tableau.com/views/TableauProject1_17525916320900/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link">Tableau</a></p>
    </div>
  </div>
</section>

<!-- Skills Section -->
<section id="skills" class="fade-in">
  <h2>Skills & Certifications</h2>
  <ul class="skills-list">
    <li>Python | Java | HTML | R | SAS | SQL</li>
    <li>Pivot Tables, Charts, MS SQL Server</li>
    <li>MTA Python | Microsoft Office Specialist | Adobe Certified Professional (Photoshop, Illustrator, Graphic Design)</li>
  </ul>
</section>

<!-- Scripts -->
<script>
/* Scroll spy for active nav links */
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

/* Fade-in animation on scroll for sections and cards */
const faders = document.querySelectorAll('.fade-in, .fade-card');
const appearOptions = { threshold: 0.1 };
const appearOnScroll = new IntersectionObserver(function(entries, appearOnScroll) {
  entries.forEach(entry => {
    if (!entry.isIntersecting) return;
    entry.target.classList.add('fade-show');
    appearOnScroll.unobserve(entry.target);
  });
}, appearOptions);
faders.forEach(el => appearOnScroll.observe(el));

/* Section heading color accent on scroll */
const headings = document.querySelectorAll('section h2');
const headingObserver = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if(entry.isIntersecting){
      entry.target.style.color = '#00a676';
    } else {
      entry.target.style.color = '';
    }
  });
}, { threshold: 0.3 });
headings.forEach(h => headingObserver.observe(h));
</script>
