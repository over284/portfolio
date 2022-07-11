<template>
    <section class="section-info">
        <div class="section-info-left">
            <div class="section-info-left-header">I have knowledge in HTML, CSS, JavaScript, Vue.js</div>
            <div class="section-info-left-desc">Also basic SASS, jQuery, Git, Photoshop</div>
            <div class="section-info-left-btn hero-video-text-btn"><a href="https://account.rabota.ua/jobsearch/cvbuilder?resumeId=20844899">More about me</a></div>
        </div>
        <div class="section-info-right"></div>
    </section>
</template>

<style>
.section-info {
    display: flex;
    height: 100vh;
    min-height: 700px;
}
.section-info-left {
    width: 50%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    padding: 120px 40px 75px 6.6%;
}
.section-info-right {
    width: 50%;
}
.section-info-left-header {
    font-size: 40px;
    line-height: 64px;
    letter-spacing: -.02em;
    font-weight: 700;
}
.section-info-left-desc {
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
.hero-video-text-btn:hover {
    background: #fd0202;
}
.section-info-right {
    background-image: url(../img/vuejs.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: 50%, 50%;
    z-index: -2;
}
</style>