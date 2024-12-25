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

<div class="carousel-container">
    <div class="carousel-slide">
        <div class="carousel-item">
            <img src="https://juliocedillo.github.io/neweconomy/assets/images/q1.png" alt="Image 1">
        </div>
        <div class="carousel-item">
            <img src="https://juliocedillo.github.io/neweconomy/assets/images/q2.png" alt="Image 2">
        </div>
        <div class="carousel-item">
            <img src="https://juliocedillo.github.io/neweconomy/assets/images/q3.png" alt="Image 3">
        </div>
        <div class="carousel-item">
            <img src="https://juliocedillo.github.io/neweconomy/assets/images/q4.png" alt="Image 4">
        </div>
        <div class="carousel-item">
            <img src="https://juliocedillo.github.io/neweconomy/assets/images/q5.png" alt="Image 5">
        </div>
    </div>
    <!-- Controls -->
    <button class="prev" onclick="moveSlide(-1)">&#10094;</button>
    <button class="next" onclick="moveSlide(1)">&#10095;</button>
</div>

<script>
let index = 0; // Track the current slide

function moveSlide(step) {
    const slides = document.querySelectorAll('.carousel-item');
    const totalSlides = slides.length;
    
    // Move to the next or previous slide
    index += step;

    if (index >= totalSlides) {
        index = 0; // Loop back to the first slide
    }
    
    if (index < 0) {
        index = totalSlides - 1; // Loop back to the last slide
    }

    // Move the carousel slide
    const carouselSlide = document.querySelector('.carousel-slide');
    carouselSlide.style.transform = `translateX(${-index * 100}%)`;
}
</script>
