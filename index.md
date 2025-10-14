---
layout: default
---

# About me
I love a project, particularly those that challenge me to solve problems and develop new skills. My journey into computer science began two years ago when I set out to automate some tasks at my previous job. I had long suspected there was a better way than bloated Excel spreadsheets but lacked the coding knowledge to make it happen. Discovering Python opened that door, and I’ve since fallen deep into the rabbit hole. This website showcases some projects I’ve built while exploring more specific areas of software and data engineering.

I'm originally from the UK and came to Christchurch, New Zealand in 2019 for a “one-year” working holiday. Six years later I’m still here and now a proud garden (and home) owner. Outside of work I enjoy building things, both digital and physical, cycling (in all forms), surfing, skiing, woodworking, and beer brewing.

I’m currently abroad on a year-long sabbatical, travelling the world with my wonderful girlfriend. After hiking in the Himalayas, exploring cultural sites in India, and cycling 3,000 km around mainland Europe, our ambitious plan continues as we cycle from Bangkok to Singapore as part of our return journey. We’ll be back in Christchurch in January 2026, when I’ll be looking for new job opportunities.

# Snaps from the road
<!-- Image Carousel -->
<div class="image-carousel">
  <div class="carousel-container">
    <img class="carousel-image active" src="/assets/img/image1.jpg" alt="Image 1">
    <img class="carousel-image" src="/assets/img/image2.jpg" alt="Image 2">
    <img class="carousel-image" src="/assets/img/image3.jpg" alt="Image 3">
    <img class="carousel-image" src="/assets/img/image4.jpg" alt="Image 4">
    <img class="carousel-image" src="/assets/img/image5.jpg" alt="Image 5">
    <img class="carousel-image" src="/assets/img/image6.jpg" alt="Image 6">
    <img class="carousel-image" src="/assets/img/image7.jpg" alt="Image 7">
    <img class="carousel-image" src="/assets/img/image8.jpg" alt="Image 8">
    <img class="carousel-image" src="/assets/img/image9.jpg" alt="Image 9">
    <img class="carousel-image" src="/assets/img/image10.jpg" alt="Image 10">
    <img class="carousel-image" src="/assets/img/image11.jpg" alt="Image 11">
  </div>
  <div class="carousel-controls">
    <button class="carousel-prev">‹</button>
    <div class="carousel-dots"></div>
    <button class="carousel-next">›</button>
  </div>
</div>

<style>
/* --- Image Carousel Styling --- */
.image-carousel {
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 850px;         /* match your page column width */
  width: 100%;              /* take full width of container */
  margin: 2rem auto;        /* center it with some breathing room */
}

.carousel-container {
  position: relative;
  width: 100%;
  aspect-ratio: 16 / 9;     /* keeps a consistent aspect ratio */
  overflow: hidden;
  border-radius: 12px;
}

.carousel-image {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;              /* match container width */
  height: 100%;             /* fill container height */
  object-fit: cover;        /* maintain aspect ratio and fill space */
  opacity: 0;
  transition: opacity 0.6s ease;
}

.carousel-image.active {
  opacity: 1;
}

.carousel-controls {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 0.5rem;
  gap: 1rem;
}

.carousel-prev,
.carousel-next {
  background: none;
  border: none;
  font-size: 2rem;
  cursor: pointer;
  color: #333;
  transition: color 0.3s ease;
}

.carousel-prev:hover,
.carousel-next:hover {
  color: #007acc;
}

/* Optional: make the dots align neatly under the images */
.carousel-dots {
  display: flex;
  gap: 0.5rem;
}

.carousel-dots button {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  border: none;
  background: #ccc;
  cursor: pointer;
}

.carousel-dots button.active {
  background: #007acc;
}

/* --- Responsive tweak --- */
@media (max-width: 900px) {
  .carousel-container {
    aspect-ratio: 4 / 3;    /* slightly taller for smaller screens */
  }
}
</style>
