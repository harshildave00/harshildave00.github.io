---
layout: default
title: Home
---

<nav class="main-nav">
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#experience">Experience</a>
  <a href="#projects">Projects</a>
</nav>

<section id="home" class="hero">
  <h1>Hi, I’m Harshil Dave</h1>
  <p class="hero-sub">
    Computer Science Student | Software Development
  </p>
</section>

<section id="about">
  <h2>About</h2>
  <p>
    I’m a Computer Science student interested in software development,
    systems, and data. I enjoy building clean, efficient projects and
    learning how systems work under the hood.
  </p>
</section>

<section id="experience">
  <h2>Experience</h2>

  <div class="item">
    <strong>Role – Company</strong><br>
    <span class="muted">Month Year – Month Year</span>
    <p>
      Brief description of what you worked on, technologies used,
      and impact.
    </p>
  </div>

  <div class="item">
    <strong>Another Role – Company</strong><br>
    <span class="muted">Month Year – Month Year</span>
    <p>
      Another short description.
    </p>
  </div>
</section>

<section id="projects">
  <h2>Projects</h2>

  <div class

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

