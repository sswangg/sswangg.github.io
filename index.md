---
layout: page
title: Coding Club
subtitle: All about the best club at Pioneer
---

<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div class="mySlides fade">
    <div class="numbertext">1 / 3</div>
    <img src="img1.jpg" style="width:100%">
    <div class="text">Caption Text</div>
  </div>

  <div class="mySlides fade">
    <div class="numbertext">2 / 3</div>
    <img src="img2.jpg" style="width:100%">
    <div class="text">Caption Two</div>
  </div>

  <div class="mySlides fade">
    <div class="numbertext">3 / 3</div>
    <img src="img3.jpg" style="width:100%">
    <div class="text">Caption Three</div>
  </div>

  <div class="mySlides fade">
    <div class="numbertext">3 / 3</div>
    <img src="img4.jpg" style="width:100%">
    <div class="text">Caption Four</div>
  </div>

  <!-- Next and previous buttons -->
  <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>
<br>

<!-- The dots/circles -->
<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span>
  <span class="dot" onclick="currentSlide(2)"></span>
  <span class="dot" onclick="currentSlide(3)"></span>
</div>
<script>
let slideIndex = 1;
showSlides(slideIndex);

// Next/previous controls
function plusSlides(n) {
  showSlides(slideIndex += n);
}

// Thumbnail image controls
function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
}
</script>

Coding Club is a club at Pioneer High School where students mess around with code, go to coding competitions, and have fun. With 50 official members and over 30 people attending every club lunch meeting, we're one of the largest clubs at Pioneer. Anyone with an interest in technology is welcome to join, and no experience is required.

One of the main focuses of the club is competitive programming, which is a mind sport where participants write programs to solve problems and are judged off of factors such as how long the program takes to run, how quickly you finish, and how much memory the program takes. Pioneer has historically had success at programming competitions like this as can be seen in this [news article](https://news.a2schools.org/pioneer-high-school-coding-team-excels-at-recent-competitions/). We **_CRUSHED_** the competiton at MSU last year too, but the details slipped away. Blame covid. 

Competitive programming isn't the pnly thing we do though. Join the club to potentially hold events teaching basic coding, meet professionals, and just learn! If this sounds interesting to you, email Sophia at 314660@aaps.k12.mi.us

Note: the [source code](https://github.com/sswangg/sswangg.github.io) for this website is publicly available.
