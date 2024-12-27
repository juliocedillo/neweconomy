---
layout: default
title: Home
permalink: /
---

<div style="position: relative; display: inline-block;">
  <img src="https://juliocedillo.github.io/neweconomy/assets/images/21.png" alt="header" style="width: 50%; height: auto; border: none;">
  <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); color: white; font-size: 24px; font-weight: bold;">
    <div align="center">
      What if the rules that defined the past 40 years of economic history were one-time, historically contingent developments that are now rapidly coming to an end?
    </div>
  </div>
</div>

Armando Lara-Millan is writing a book tentatively titled The Firm That Predicted the Future and the Birth of a New Global Economy. It argues that over the past forty years, five global political-economic dynamics were largely mistaken for the new, permanent rules of the globalized economy. Instead, they were one-time, historically contingent developments that are now rapidly changing. Pairing a qualitative study of a key investment firm with the natural language processing of decades of corporate quarterly reports, Lara-Millan details the end of low-cost labor in China, the transition from high-growth to cyclical internet-beneficiary sectors, the move from cheap energy to expensive raw materials, the inability to further lower corporate taxes and the cost of corporate borrowing, and the uncertain role of performative monetary policy. The book offers a way of making sense of our supposed “polycrisis” to understand better how a new order is struggling to be born in the present.

---

|Goal|Method|Impact|
|---|---|---|
|Our project investigates the end of low-cost labor in China and easy money in Silicon Valley, desperate explorations for copper and lithium deposits on old oil and coal fields, to the language games of Central Bankers in Jackson Hole and the European Central Bank.| Weaving ethnographies of key asset management firms, interviews with employers and employees in key sectors across the world, and natural language processing of decades of quarterly reports from every major corporation, the Future of the Global Economy project is working to understand how a new global order is struggling to be born in the present. | Historicizing the past 40 years weaves together disparate arguments about “neoliberalism,” “financialization,” and “hyper globalization.” As such, we hope to make sense of our contemporary “polycrisis” and understand how a new global order is struggling to be born in the present. |

---

<p>&nbsp;&nbsp;&nbsp;</p>

<h2 style="text-align: center;">Dynamics We're Investigating</h2>

<!-- HTML for the Carousel -->
<div class="carousel">
  <div class="carousel-container">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q1.png" alt="Image 1">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q2.png" alt="Image 2">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q3.png" alt="Image 3">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q4.png" alt="Image 4">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q5.png" alt="Image 5">
  </div>
  <button class="carousel-prev" onclick="moveSlide(-1)">&#10094;</button>
  <button class="carousel-next" onclick="moveSlide(1)">&#10095;</button>
</div>

<!-- CSS for styling the Carousel -->
<style>
  .carousel {
    position: relative;
    max-width: 800px; /* Adjust width as necessary */
    margin: auto;
    overflow: hidden;
  }

  .carousel-container {
    display: flex;
    transition: transform 0.5s ease;
  }

  .carousel-slide {
    width: 100%;
    flex-shrink: 0; /* Prevents the images from shrinking */
    display: block;
  }

  .carousel-prev, .carousel-next {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    color: white;
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

<!-- JavaScript to control the Carousel -->
<script>
  let currentIndex = 0;

  // Function to move the slide
  function moveSlide(direction) {
    const slides = document.querySelectorAll('.carousel-slide');
    const totalSlides = slides.length;

    // Update the currentIndex based on direction
    currentIndex = (currentIndex + direction + totalSlides) % totalSlides;

    // Update the position of the carousel container
    document.querySelector('.carousel-container').style.transform = `translateX(-${currentIndex * 100}%)`;
  }
</script>
