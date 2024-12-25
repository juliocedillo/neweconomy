---
layout: default
title: Home
permalink: /
---

<div align="center">
  What if the rules that defined the past 40 years of economic history were one-time, historically contingent developments that are now rapidly coming to an end?
</div>

<p>&nbsp;&nbsp;&nbsp;</p>

---

|Goal|Method|Impact|
|---|---|---|
|Our project investigates the end of low-cost labor in China and easy money in Silicon Valley, desperate explorations for copper and lithium deposits on old oil and coal fields, to the language games of Central Bankers in Jackson Hole and the European Central Bank.| Weaving ethnographies of key asset management firms, interviews with employers and employees in key sectors across the world, and natural language processing of decades of quarterly reports from every major corporation, the Future of the Global Economy project is working to understand how a new global order is struggling to be born in the present. | Historicizing the past 40 years weaves together disparate arguments about “neoliberalism,” “financialization,” and “hyper globalization.” As such, we hope to make sense of our contemporary “polycrisis” and understand how a new global order is struggling to be born in the present. |

---

<p>&nbsp;&nbsp;&nbsp;</p>

<h2 style="text-align: center;">Dynamics We're Investigating</h2>

<!-- HTML for the Carousel-->
<div class="carousel">
  <div class="carousel-container">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q1.png">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q2.png">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q3.png">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q4.png">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q5.png">
  </div>
  <button class="carousel-prev" onclick="moveSlide(-1)">&#10094;</button>
  <button class="carousel-next" onclick="moveSlide(1)">&#10095;</button>
</div>

<!-- CSS Styling -->
<style>
  .carousel {
    position: relative;
    max-width: 800px;
    margin: auto;
    overflow: hidden;
  }

  .carousel-container {
    display: flex;
    transition: transform 0.5s ease;
  }

  .carousel-slide {
    width: 100%
    display: block;
  }

  .carousel-prev, .carousel-next {
    position: absolute;
    top: 50%
    transform: translateY(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    color: white
    border: none;
    padding: 16px;
    cursor: pointer;
    z-index: 10;
  }

  .carousel-prev {
    left: 0;
  }

  .carousel-next {
    right: 0;
  }
</style>

<!-- JS Control -->
<script>
  let currentIndex = 0;

  funcion moveSlide(direction) {
    const slides = document.querySelectorAll('.carousel-slide');
    const totalSlides = slides.length;

    currentIndex = (currentIndex + direction + totalSlides) % totalSlides;
    document.querySelector('.carousel-containter').style.transform = `translateX(-${currentIndex * 100}%)`;
  }
</script>

