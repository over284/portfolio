<template>
<section class="section-third-info">
    <div class="section-third-info-left">
        <div class="section-third-info-left-header">This is my first work done in wordpress</div>
        <div class="section-third-info-left-desc">The site was made using the elementor plugin</div>
        <div class="section-third-info-left-btn hero-video-text-btn"><a href="https://github.com/over284?tab=repositories">All works</a></div>
    </div>
    <div class="section-third-info-right">
        <carousel>
            <carousel-slide v-for="slide in slides" :key="slide" class="carousel-slider">
                <img :src="slide" :alt="slide">
            </carousel-slide>
        </carousel>
    </div>
</section>
</template>

<style>
.section-third-info {
    display: flex;
    height: 100vh;
    min-height: 700px;
}

.section-third-info-left {
    width: 50%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    padding: 120px 40px 75px 6.6%;
}

.section-third-info-right {
    width: 60%;
}

.section-third-info-left-header {
    font-size: 40px;
    line-height: 64px;
    letter-spacing: -.02em;
    font-weight: 700;
}

.section-third-info-left-desc {
    margin-top: 15px;
    font-size: 24px;
    line-height: 36px;
    letter-spacing: -.03em;
    font-weight: 400;
    color: #828282;
}

.hero-video-text-btn {
    margin-top: 30px;
    display: inline-block;
    padding: 14px 34px;
    font-size: 16px;
    border: 2px solid #fd0202;
    border-radius: 4px;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
    text-align: center;
    transition: background .3s ease-in-out;
    cursor: pointer;
}
.hero-video-text-btn a{
    text-decoration: none;
    color: #fff;
}
.hero-video-text-btn:hover {
    background: #fd0202;
}

.section-third-info-right {
    display: flex;
    justify-content: center;
    padding-right: 15px;
}

.carousel {
    position: relative;
    overflow: hidden;
    width: 1000px;
    height: 100vh;
    z-index: 10;
    background-color: rgb(0, 0, 0);
}

.btn {
    padding: 5px 10px;
    background-color: rgba(0, 0, 0, 0.5);
    border: 1px solid transparent;
    margin: 5px 10px;
    color: #FFF;
    height: 50px;
    width: 50px;
    position: absolute;
    margin-top: -25px;
    z-index: 2;
}

.btn:hover {
    cursor: pointer;
}

.btn:focus {
    outline: none;
}

.btn-next {
    top: 50%;
    right: 0;
}

.btn-prev {
    top: 50%;
    left: 0;
}

.carousel-slider {
    position: absolute;
    top: 15%;
    left: 0;
    bottom: 0;
    right: 0;
}

.carousel-slider img {
    width: 100%;
    height: 80%;
}
</style>

<script>
import Carousel from './myCarousel.vue';
import CarouselSlide from './myCarouselSlide.vue';
import img1 from '../img/1.png';
import img2 from '../img/2.png';
import img3 from '../img/3.png';
export default {
    data() {
        return {
            slides: [
                img1,
                img2,
                img3,
            ]
        }
    },
    components: {
        Carousel: Carousel,
        CarouselSlide: CarouselSlide,
    }
}
</script>
