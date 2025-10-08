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
  margin: 0.5rem auto;
  max-width: 850px;
  padding: 0.5rem;
}

.projects-landing h1 {
  font-size: 2em;
  margin-bottom: 1rem;
  color: #222;
}

.projects-landing p {
  font-size: 1.2rem;
  color: #555;
  margin-bottom: 3rem;
}

.project-links {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 0.5rem;
}

.project-card {
  background: #f9f9f9;
  border-radius: 0.5rem;
  padding: 0.5rem;
  width: 550px;
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
  font-size: 3rem;
  color: #0277b3ff;
  margin-bottom: 0.5rem;
}

.project-card h2 {
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
}

.project-card a {
  text-decoration: none;
  color: inherit;
}

.project-card p {
  color: #666;
  font-size: 1rem;
  margin-bottom: 0; /* ✅ remove bottom gap */
}

/* --- Responsive for phones --- */
@media (max-width: 600px) {
  .project-card {
    width: 90%; /* reduce width on small screens */
    max-width: 300px; /* optional, caps the max width */
  }
}
</style>

<!-- Include Font Awesome (for icons) -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<div class="projects-landing">
  <h1 style="display:inline; margin-right:10px;">Projects</h1>
  <p style="display:inline;">Explore what I’ve been working on:</p>
</div>

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


