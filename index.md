---
layout: default
---

<style>
.image-carousel {
  position: relative;
  width: 100%;
  max-width: 800px;
  margin: 1.5rem auto;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.12);
  background: transparent; /* removes grey flashes */
}

/* Carousel container: fill width, maintain 3:2 ratio */
.carousel-container {
  display: flex;
  width: 100%;
  height: auto;
  aspect-ratio: 3 / 2;
  transition: transform 0.5s ease;
  background: transparent;
}

/* Images: fill container completely */
.carousel-image {
  flex-shrink: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  margin: 0;
  padding: 0;
  border: none;
  background: transparent;
}

/* Controls sit just inside bottom edge */
.carousel-controls {
  position: absolute;
  inset: 0;
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
  padding: 0 8px 8px;
  pointer-events: none;
  z-index: 5;
}

.carousel-controls button {
  background: rgba(0,0,0,0.45);
  color: #fff;
  border: none;
  border-radius: 50%;
  width: 36px;
  height: 36px;
  font-size: 1.3rem;
  line-height: 1;
  cursor: pointer;
  pointer-events: auto;
  transition: background 0.3s ease, transform 0.2s ease;
}

.carousel-controls button:hover {
  background: rgba(0,0,0,0.7);
  transform: scale(1.1);
}

/* Dots */
.carousel-dots {
  position: absolute;
  bottom: 8px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  gap: 8px;
  z-index: 4;
}

.carousel-dots span {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: rgba(255,255,255,0.6);
  cursor: pointer;
  transition: background 0.3s;
}

.carousel-dots span.active {
  background: white;
}

/* --- Responsive tweaks --- */
@media (max-width: 800px) {
  .image-carousel {
    max-width: 100%; /* let carousel fill viewport */
    border-radius: 0; /* optional for edge-to-edge mobile look */
  }

  .carousel-container {
    aspect-ratio: auto; /* let height adjust naturally */
    height: auto;
  }

  .carousel-image {
    width: 100%;
    height: auto;
  }
}

@media (max-width: 600px) {
  .carousel-controls button {
    width: 30px;
    height: 30px;
    font-size: 1.1rem;
  }
}
</style>

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
