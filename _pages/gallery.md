---
layout: single
title: "Gallery"
permalink: /gallery/
author_profile: true
---

<p style="font-style: italic; color: #555; margin-bottom: 20px;">Highlights and snapshots from recent events and research activities. Swipe, use arrows, or watch the slides auto-play in random order.</p>

<div class="slideshow-container" id="slideshow">

  <!-- Slide 1 -->
  <div class="mySlides fade">
    <div class="numbertext">1 / 17</div>
    <img src="/images/873B853E-5CD9-4E5B-BB38-6139B0651B59.jpg" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Research and Community Highlight</div>
  </div>

  <!-- Slide 2 -->
  <div class="mySlides fade">
    <div class="numbertext">2 / 17</div>
    <img src="/images/A7303616.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Event Snapshot</div>
  </div>

  <!-- Slide 3 -->
  <div class="mySlides fade">
    <div class="numbertext">3 / 17</div>
    <img src="/images/A7303633.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Research Presentation</div>
  </div>

  <!-- Slide 4 -->
  <div class="mySlides fade">
    <div class="numbertext">4 / 17</div>
    <img src="/images/A7303674.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Community Engagement</div>
  </div>

  <!-- Slide 5 -->
  <div class="mySlides fade">
    <div class="numbertext">5 / 17</div>
    <img src="/images/CHYSresearch-1.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">CHYS Research Session</div>
  </div>

  <!-- Slide 6 -->
  <div class="mySlides fade">
    <div class="numbertext">6 / 17</div>
    <img src="/images/CHYSresearch-4.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">CHYS Research Showcase</div>
  </div>

  <!-- Slide 7 -->
  <div class="mySlides fade">
    <div class="numbertext">7 / 17</div>
    <img src="/images/CHYSresearch-8.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">CHYS Team Discussion</div>
  </div>

  <!-- Slide 8 -->
  <div class="mySlides fade">
    <div class="numbertext">8 / 17</div>
    <img src="/images/F0F809B5-6D35-4988-8F04-A6B2171686F0.jpg" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Academic Conference</div>
  </div>

  <!-- Slide 9 -->
  <div class="mySlides fade">
    <div class="numbertext">9 / 17</div>
    <img src="/images/IMG_0871.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Project Snapshot</div>
  </div>

  <!-- Slide 10 -->
  <div class="mySlides fade">
    <div class="numbertext">10 / 17</div>
    <img src="/images/IMG_3628.jpg" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Participant Interaction</div>
  </div>

  <!-- Slide 11 -->
  <div class="mySlides fade">
    <div class="numbertext">11 / 17</div>
    <img src="/images/IMG_4162.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Workshop Event</div>
  </div>

  <!-- Slide 12 -->
  <div class="mySlides fade">
    <div class="numbertext">12 / 17</div>
    <img src="/images/IMG_4163.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Group Activity</div>
  </div>

  <!-- Slide 13 -->
  <div class="mySlides fade">
    <div class="numbertext">13 / 17</div>
    <img src="/images/IMG_4167.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Panel Discussion</div>
  </div>

  <!-- Slide 14 -->
  <div class="mySlides fade">
    <div class="numbertext">14 / 17</div>
    <img src="/images/IMG_4170.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Seminar Overview</div>
  </div>

  <!-- Slide 15 -->
  <div class="mySlides fade">
    <div class="numbertext">15 / 17</div>
    <img src="/images/img7.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Fieldwork Moment</div>
  </div>

  <!-- Slide 16 -->
  <div class="mySlides fade">
    <div class="numbertext">16 / 17</div>
    <img src="/images/img8.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Community Engagement</div>
  </div>

  <!-- Next and previous buttons -->
  <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>

<!-- The dots container (dynamically generated for random count) -->
<div id="dots-container" style="text-align:center; margin-top: 15px;"></div>

<script>
  let slideIndex = 1;
  let autoSlideTimer = null;
  let slides = [];

  window.addEventListener('DOMContentLoaded', (event) => {
    let container = document.getElementById('slideshow');
    let slideElements = Array.from(container.getElementsByClassName('mySlides'));
    
    // Show the first slide immediately so it's never blank on load
    if (slideElements.length > 0) {
      slideElements[0].style.display = "block";
    }

    // Randomize the order of slides array
    slideElements.sort(() => Math.random() - 0.5);
    
    // Re-append them in random order and update number texts
    slideElements.forEach((slide, index) => {
      container.appendChild(slide);
      let numText = slide.getElementsByClassName('numbertext')[0];
      if(numText) {
        numText.innerText = (index + 1) + " / " + slideElements.length;
      }
    });

    slides = slideElements;
    
    // Build dots dynamically based on shuffled length
    let dotsContainer = document.getElementById('dots-container');
    slides.forEach((_, index) => {
      let dot = document.createElement('span');
      dot.className = 'dot';
      dot.onclick = function() { currentSlide(index + 1); };
      dotsContainer.appendChild(dot);
    });

    showSlides(slideIndex);
    startAutoSlide();
  });

  function plusSlides(n) {
    clearTimeout(autoSlideTimer);
    showSlides(slideIndex += n);
    startAutoSlide();
  }

  function currentSlide(n) {
    clearTimeout(autoSlideTimer);
    showSlides(slideIndex = n);
    startAutoSlide();
  }

  function showSlides(n) {
    if (slides.length === 0) return;
    if (n > slides.length) { slideIndex = 1; }
    if (n < 1) { slideIndex = slides.length; }
    
    for (let i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
    }
    
    let dots = document.getElementsByClassName("dot");
    for (let i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
    }
    
    slides[slideIndex - 1].style.display = "block";
    if (dots[slideIndex - 1]) {
      dots[slideIndex - 1].className += " active";
    }
  }

  function startAutoSlide() {
    autoSlideTimer = setTimeout(function() {
      slideIndex++;
      if (slideIndex > slides.length) { slideIndex = 1; }
      showSlides(slideIndex);
      startAutoSlide();
    }, 4000); // Changes image every 4 seconds
  }
</script>

<style>
  /* Page title global matching styles */
  .page__title {
    color: #1a237e !important;
    font-weight: 800 !important;
    border-bottom: 2px solid #d84315 !important;
    padding-bottom: 4px !important;
  }

  /* Slideshow container styles */
  .slideshow-container {
    max-width: 700px;
    position: relative;
    margin: auto;
    background: rgba(255, 255, 255, 0.4);
    border: 1px solid #dcd6cd;
    border-radius: 8px;
    padding: 10px;
    box-sizing: border-box;
  }

  .mySlides {
    display: none;
  }

  /* Next & previous buttons */
  .prev, .next {
    cursor: pointer;
    position: absolute;
    top: 50%;
    width: auto;
    padding: 16px;
    margin-top: -22px;
    color: white;
    font-weight: bold;
    font-size: 18px;
    transition: 0.6s ease;
    border-radius: 0 3px 3px 0;
    user-select: none;
    background-color: rgba(0,0,0,0.4);
  }

  .next {
    right: 10px;
    border-radius: 3px 0 0 3px;
  }
  
  .prev {
    left: 10px;
  }

  .prev:hover, .next:hover {
    background-color: rgba(0,0,0,0.8);
  }

  /* Caption text */
  .text {
    color: #333;
    font-size: 0.95rem;
    padding: 10px 12px;
    position: absolute;
    bottom: 8px;
    width: 100%;
    text-align: center;
    background: rgba(255, 255, 255, 0.85);
    border-bottom-left-radius: 8px;
    border-bottom-right-radius: 8px;
    box-sizing: border-box;
  }

  .numbertext {
    color: #f2f2f2;
    font-size: 12px;
    padding: 8px 12px;
    position: absolute;
    top: 0;
    background: rgba(0,0,0,0.4);
    border-top-left-radius: 8px;
  }

  /* The dots/bullets/indicators */
  .dot {
    cursor: pointer;
    height: 12px;
    width: 12px;
    margin: 0 4px;
    background-color: #bbb;
    border-radius: 50%;
    display: inline-block;
    transition: background-color 0.6s ease;
  }

  .active, .dot:hover {
    background-color: #d84315;
  }

  /* Fading animation */
  .fade {
    animation-name: fade;
    animation-duration: 1.5s;
  }

  @keyframes fade {
    from {opacity: .4}
    to {opacity: 1}
  }
</style>
