<template>
<section class="hero-video">
    <video class="hero-bg-video" muted autoplay loop>
        <source src="../img/design1.mp4">
    </video>
    <div class="hero-video-text">
        <h1 class="hero-video-text-h1">I'm Stepanets Vadim, a<br>
            begginer front-end developer</h1>
        <!-- <div class="hero-video-text-btn">Learn more</div> -->

    </div>
    <div class="hero-video-mouse">
        <div class="mouse"></div>
    </div>

</section>
</template>

<style>
.hero-video {
    display: flex;
    width: 100%;
    height: 100vh;
    /* min-height: 700px; */
}

.hero-bg-video {
    width: 100%;
    height: 100%;
    left: 0%;
    top: 0%;
    position: absolute;
    object-fit: cover;
    z-index: -2;
}

.hero-video::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    left: 0%;
    top: 0%;
    z-index: -1;
    background: #000;
    opacity: .7;
}

.hero-video-text {
    position: absolute;
    top: 450px;
    bottom: 0;
    padding: 120px 40px 75px 6.6%;
    text-align: left;
     font-size: 16px;
}

/* .hero-video-text-btn {
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

.hero-video-text-btn:hover {
    background: #fd0202;
} */
.hero-video-mouse{
    position: absolute;
    top: auto;
    bottom: 20px;
    padding: 0% 50% 0% 50%;
    text-align: center;
}
.mouse {
    width: 30px;
    height: 50px;
    border: 2px solid #ffffff;
    border-radius: 60px;
    position: relative;
    box-sizing: border-box;
}

.mouse::before {
    content: '';
    width: 12px;
    height: 12px;
    position: absolute;
    top: 10px;
    left: 50%;
    transform: translateX(-50%);
    background-color: #ffffff;
    border-radius: 50%;
    opacity: 1;
    animation: wheel 2s infinite;
}

@keyframes wheel {
    to {
        opacity: 0;
        top: 40px;
    }
}
</style>
