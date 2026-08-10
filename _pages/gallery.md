---
layout: single
title: "Gallery"
permalink: /gallery/
author_profile: true
---

<p style="font-style: italic; color: #555; margin-bottom: 20px;">Highlights and snapshots from recent events and research activities. Use the arrows to navigate through the slides.</p>

<div class="slideshow-container">

  <!-- Slide 1 (Active by default so it never loads blank) -->
  <div class="mySlides fade" style="display: block;">
    <div class="numbertext">1 / 16</div>
    <img src="/images/873B853E-5CD9-4E5B-BB38-6139B0651B59.jpg" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Research and Community Highlight</div>
  </div>

  <!-- Slide 2 -->
  <div class="mySlides fade">
    <div class="numbertext">2 / 16</div>
    <img src="/images/A7303616.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Event Snapshot</div>
  </div>

  <!-- Slide 3 -->
  <div class="mySlides fade">
    <div class="numbertext">3 / 16</div>
    <img src="/images/A7303633.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Research Presentation</div>
  </div>

  <!-- Slide 4 -->
  <div class="mySlides fade">
    <div class="numbertext">4 / 16</div>
    <img src="/images/A7303674.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Community Engagement</div>
  </div>

  <!-- Slide 5 -->
  <div class="mySlides fade">
    <div class="numbertext">5 / 16</div>
    <img src="/images/CHYSresearch-1.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">CHYS Research Session</div>
  </div>

  <!-- Slide 6 -->
  <div class="mySlides fade">
    <div class="numbertext">6 / 16</div>
    <img src="/images/CHYSresearch-4.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">CHYS Research Showcase</div>
  </div>

  <!-- Slide 7 -->
  <div class="mySlides fade">
    <div class="numbertext">7 / 16</div>
    <img src="/images/CHYSresearch-8.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">CHYS Team Discussion</div>
  </div>

  <!-- Slide 8 -->
  <div class="mySlides fade">
    <div class="numbertext">8 / 16</div>
    <img src="/images/F0F809B5-6D35-4988-8F04-A6B2171686F0.jpg" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Academic Conference</div>
  </div>

  <!-- Slide 9 -->
  <div class="mySlides fade">
    <div class="numbertext">9 / 16</div>
    <img src="/images/IMG_0871.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Project Snapshot</div>
  </div>

  <!-- Slide 10 -->
  <div class="mySlides fade">
    <div class="numbertext">10 / 16</div>
    <img src="/images/IMG_3628.jpg" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Participant Interaction</div>
  </div>

  <!-- Slide 11 -->
  <div class="mySlides fade">
    <div class="numbertext">11 / 16</div>
    <img src="/images/IMG_4162.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Workshop Event</div>
  </div>

  <!-- Slide 12 -->
  <div class="mySlides fade">
    <div class="numbertext">12 / 16</div>
    <img src="/images/IMG_4163.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Group Activity</div>
  </div>

  <!-- Slide 13 -->
  <div class="mySlides fade">
    <div class="numbertext">13 / 16</div>
    <img src="/images/IMG_4167.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Panel Discussion</div>
  </div>

  <!-- Slide 14 -->
  <div class="mySlides fade">
    <div class="numbertext">14 / 16</div>
    <img src="/images/IMG_4170.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Seminar Overview</div>
  </div>

  <!-- Slide 15 -->
  <div class="mySlides fade">
    <div class="numbertext">15 / 16</div>
    <img src="/images/img7.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Fieldwork Moment</div>
  </div>

  <!-- Slide 16 -->
  <div class="mySlides fade">
    <div class="numbertext">16 / 16</div>
    <img src="/images/img8.JPG" alt="Highlight" style="width:100%; border-radius: 8px;">
    <div class="text">Community Engagement</div>
  </div>

  <!-- Next and previous buttons -->
  <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>

<!-- The dots/circles -->
<div style="text-align:center; margin-top: 15px;">
  <span class="dot" onclick="currentSlide(1)"></span>
  <span class="dot" onclick="currentSlide(2)"></span>
  <span class="dot" onclick="currentSlide(3)"></span>
  <span class="dot" onclick="currentSlide(4)"></span>
  <span class="dot" onclick="currentSlide(5)"></span>
  <span class="dot" onclick="currentSlide(6)"></span>
  <span class="dot" onclick="currentSlide(7)"></span>
  <span class="dot" onclick="currentSlide(8)"></span>
  <span class="dot" onclick="currentSlide(9)"></span>
  <span class="dot" onclick="currentSlide(10)"></span>
  <span class="dot" onclick="currentSlide(11)"></span>
  <span class="dot" onclick="currentSlide(12)"></span>
  <span class="dot" onclick="currentSlide(13)"></span>
  <span class="dot" onclick="currentSlide(14)"></span>
  <span class="dot" onclick="currentSlide(15)"></span>
  <span class="dot" onclick="currentSlide(16)"></span>
</div>

<script>
  let slideIndex = 1;
  let autoSlideTimer = null;

  showSlides(slideIndex);
  startAutoSlide();

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
    let slides = document.getElementsByClassName("mySlides");
    let dots = document.getElementsByClassName("dot");
    if (n > slides.length) { slideIndex = 1; }
    if (n < 1) { slideIndex = slides.length; }
    
    for (let i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
    }
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
      let slides = document.getElementsByClassName("mySlides");
      if (slideIndex > slides.length) { slideIndex = 1; }
      showSlides(slideIndex);
      startAutoSlide();
    }, 4000);
  }
</script>

<style>
  .page__title {
    color: #1a237e !important;
    font-weight: 800 !important;
    border-bottom: 2px solid #d84315 !important;
    padding-bottom: 4px !important;
  }

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
    z-index: 10;
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
    z-index: 5;
  }

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

  .fade {
    animation-name: fade;
    animation-duration: 1.5s;
  }

  @keyframes fade {
    from {opacity: .4}
    to {opacity: 1}
  }
</style>
