---
layout: default
title: Projects
permalink: /projects/
---

<style>
/* --- Projects Landing Page Styling --- */
.projects-landing {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  margin: 4rem auto;
  max-width: 850px;
  padding: 1rem;
}

/* Match the site's normal Markdown H1 size */
.projects-landing h1 {
  font-size: 2em; /* same as Markdown # heading */
  font-weight: 700;
  margin-bottom: 1rem;
  color: #222;
}

.projects-landing p {
  font-size: 1.1rem;
  color: #555;
  margin-bottom: 2.5rem;
  max-width: 700px;
}

/* Two cards side by side, centered, max combined width 850px */
.project-links {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
  max-width: 850px;
}

.project-card {
  background: #f9f9f9;
  border-radius: 1rem;
  padding: 2rem;
  width: 100%;
  max-width: 400px; /* two cards fit side by side within 850px total */
  text-align: center;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  transition: all 0.3s ease;
}

.project-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
  background: #fff;
}

.project-card i {
  font-size: 2.5rem;
  color: #2a9d8f;
  margin-bottom: 1rem;
}

.project-card h2 {
  font-size: 1.4rem;
  margin-bottom: 0.5rem;
}

.project-card a {
  text-decoration: none;
  color: inherit;
}

.project-card p {
  color: #666;
  font-size: 1rem;
}
</style>

<!-- Include Font Awesome (for icons) -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<div class="projects-landing">
  <h1>Projects</h1>
  <p>Explore what I’ve been working on, from software experiments to hands-on DIY builds</p>

  <div class="project-links">
    <a href="/projects/software/" class="project-card">
      <i class="fa-solid fa-laptop-code"></i>
      <h2>Software</h2>
      <p>Apps, tools, and data-driven experiments</p>
    </a>

    <a href="/projects/diy/" class="project-card">
      <i class="fa-solid fa-hammer"></i>
      <h2>DIY</h2>
      <p>Campervan builds, gardening, woodworking, and other creative weekend projects</p>
    </a>
  </div>
</div>
