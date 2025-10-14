---
layout: default
---

<style>
/* Carousel Styles */
.image-carousel {
  max-width: 850px;
  width: 100%;
  margin: 0 auto;
}

.carousel-container {
  position: relative;
  width: 100%;
  height: 0;
  padding-bottom: 66.67%; /* 3:2 aspect ratio - better for photos */
  overflow: hidden;
  border-radius: 8px;
}

.carousel-image {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0;
  transition: opacity 0.5s ease-in-out;
}

.carousel-image.active {
  opacity: 1;
}

.carousel-controls {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
  margin-top: 15px;
  padding: 0 10px;
}

.carousel-prev,
.carousel-next {
  background: rgba(0, 0, 0, 0.7);
  color: white;
  border: none;
  border-radius: 50%;
  width: 40px;
  height: 40px;
  font-size: 20px;
  cursor: pointer;
  transition: background 0.3s ease;
  flex-shrink: 0;
}

.carousel-prev:hover,
.carousel-next:hover {
  background: rgba(0, 0, 0, 0.9);
}

.carousel-dots {
  display: flex;
  gap: 8px;
  flex-wrap: wrap;
  justify-content: center;
}

.carousel-dots .dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #ccc;
  cursor: pointer;
  transition: background 0.3s ease;
  flex-shrink: 0;
}

.carousel-dots .dot.active {
  background: #333;
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const images = document.querySelectorAll('.carousel-image');
  const prevButton = document.querySelector('.carousel-prev');
  const nextButton = document.querySelector('.carousel-next');
  const dotsContainer = document.querySelector('.carousel-dots');
  
  let currentIndex = 0;
  
  // Clear any existing dots first (in case of page refresh issues)
  dotsContainer.innerHTML = '';
  
  // Create dots - ONLY once per image
  images.forEach((_, index) => {
    const dot = document.createElement('div');
    dot.classList.add('dot');
    if (index === 0) dot.classList.add('active');
    dot.addEventListener('click', () => goToSlide(index));
    dotsContainer.appendChild(dot);
  });
  
  const dots = document.querySelectorAll('.dot');
  
  function goToSlide(index) {
    // Remove active class from current image and dot
    images[currentIndex].classList.remove('active');
    if (dots[currentIndex]) {
      dots[currentIndex].classList.remove('active');
    }
    
    currentIndex = index;
    
    // Add active class to new image and dot
    images[currentIndex].classList.add('active');
    if (dots[currentIndex]) {
      dots[currentIndex].classList.add('active');
    }
  }
  
  function nextSlide() {
    const nextIndex = (currentIndex + 1) % images.length;
    goToSlide(nextIndex);
  }
  
  function prevSlide() {
    const prevIndex = (currentIndex - 1 + images.length) % images.length;
    goToSlide(prevIndex);
  }
  
  prevButton.addEventListener('click', prevSlide);
  nextButton.addEventListener('click', nextSlide);
  
  // Optional: Auto-advance every 5 seconds
  // let carouselInterval = setInterval(nextSlide, 5000);
  
  // Optional: Pause auto-advance on hover
  // const carousel = document.querySelector('.image-carousel');
  // carousel.addEventListener('mouseenter', () => clearInterval(carouselInterval));
  // carousel.addEventListener('mouseleave', () => {
  //   carouselInterval = setInterval(nextSlide, 5000);
  // });
});
</script>

# About me
I love a project, particularly those that challenge me to solve problems and develop new skills. My journey into computer science began two years ago when I set out to automate some tasks at my previous job. I had long suspected there was a better way than bloated Excel spreadsheets but lacked the coding knowledge to make it happen. Discovering Python opened that door, and I've since fallen deep into the rabbit hole. This website showcases some projects I've built while exploring more specific areas of software and data engineering.

I'm originally from the UK and came to Christchurch, New Zealand in 2019 for a "one-year" working holiday. Six years later I'm still here and now a proud garden (and home) owner. Outside of work I enjoy building things, both digital and physical, cycling (in all forms), surfing, skiing, woodworking, and beer brewing.

I'm currently abroad on a year-long sabbatical, travelling the world with my wonderful girlfriend. After hiking in the Himalayas, exploring cultural sites in India, and cycling 3,000 km around mainland Europe, our ambitious plan continues as we cycle from Bangkok to Singapore as part of our return journey. We'll be back in Christchurch in January 2026, when I'll be looking for new job opportunities.

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