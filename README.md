This website was made for Professor [Armando Lara-Millán]("https://sociology.berkeley.edu/faculty/armando-lara-millan") for his upcoming research project. 

Use this for later:

# Welcome to My GitHub Page!

## Image Carousel

<div class="carousel-container">
    <div class="carousel-slide">
        <div class="carousel-item">
            <img src="images/image1.jpg" alt="Image 1">
        </div>
        <div class="carousel-item">
            <img src="images/image2.jpg" alt="Image 2">
        </div>
        <div class="carousel-item">
            <img src="images/image3.jpg" alt="Image 3">
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

## More Content Here
Feel free to add more content below the carousel.

