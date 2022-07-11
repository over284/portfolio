<template>
<section class="hero-video-five">
    <video class="hero-bg-video-five" muted autoplay loop>
        <source src="../img/design.mp4">
    </video>
    <div class="hero-video-text-five">
        <div class="five-section-info-left-header">I am sociable, attentive, responsible, creative</div>
            <div class="five-section-info-left-desc">I have a great desire to work and develop, to gain practical skills</div>
        <!-- <div class="hero-video-text-btn">Learn more</div> -->
         </div>
</section>
</template>

<style>
.hero-video-five{
    display: flex;
    width: 100%;
    height: 100vh;
}
.hero-bg-video-five {
    width: 100%;
    height: 100%;
    position: absolute;
    object-fit: cover;
    z-index: -2;
}
.hero-video-five::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    z-index: -1;
    background: #000;
    opacity: .7;
}
/* .hero-video-text-five {
    width: 700px;
    margin-top: 400px;
    padding: 120px 0px 0px 6.6%;
    text-align: left;
    font-size: 20px;
} */
.five-section-info-left-header {
    width: 600px;
    margin-top: 400px;
    padding-left: 120px;
    font-size: 30px;
    line-height: 44px;
    letter-spacing: -.02em;
    font-weight: 700;
}
.five-section-info-left-desc {
    width: 600px;
    padding-left: 120px;
    margin-top: 15px;
    font-size: 24px;
    line-height: 36px;
    letter-spacing: -.03em;
    font-weight: 400;
    color: #828282;
}
</style>