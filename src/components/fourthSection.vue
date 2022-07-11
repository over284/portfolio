<template>
    <section class="fourth-section-info">
        <div class="fourth-section-info-left">
            <div class="fourth-section-info-left-header">I am currently working on Vue.js and studying it in depth</div>
            <div class="fourth-section-info-left-desc">In parallel with this, i learn the SASS preprocessor</div>
            <!-- <div class="fourth-section-info-left-btn hero-video-text-btn">More about me</div> -->
        </div>
        <div class="fourth-section-info-right"></div>
    </section>
</template>

<style>
.fourth-section-info {
    display: flex;
    height: 100vh;
    min-height: 700px;
}
.fourth-section-info-left {
    width: 50%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    padding: 120px 40px 75px 6.6%;
}
.fourth-section-info-right {
    width: 50%;
}
.fourth-section-info-left-header {
    font-size: 40px;
    line-height: 64px;
    letter-spacing: -.02em;
    font-weight: 700;
}
.fourth-section-info-left-desc {
    margin-top: 15px;
    font-size: 24px;
    line-height: 36px;
    letter-spacing: -.03em;
    font-weight: 400;
    color: #828282;
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
.fourth-section-info-right {
    background-image: url(../img/sass.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: 50%, 50%;
    z-index: -2;
}
</style>