<template>
<div class="preloader">
    <div class="preloader-logo">JkSite</div>
</div>
</template>

<style>
.preloader {
    position: fixed;
    top: 0;
    left: 0;
    background: #000;
    color: #fff;
    width: 100%;
    height: 100%;
    z-index: 999999;
    display: flex;
    justify-content: center;
    align-items: center;
    animation: slide-fade 1s ease-in-out forwards;
    animation-delay: 3s;
    z-index: 999999999;
}


.preloader-logo {
    padding-left: 5px;
    font-size: 60px;
    animation: zoom 1s ease-in-out forwards;
    transform: scale(1);
    position: relative;
    overflow: hidden;
}

@keyframes zoom {
    0% {
        transform: scale(1);
    }
    100% {
        transform: scale(1.2);
    }
}

@keyframes slide-right {
    0% {
        transform: translateX(-110%);
    }
    50% {
        transform: translateX(0%);
    }
    100% {
        transform: translateX(140%);
    }
    
}

@keyframes slide-fade {
    0% {
        transform: translateX(0%);
    }
    100% {
        transform: translateX(110%);
    }
    
}

.preloader-logo::before {
    position: absolute;
    content: "";
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: aliceblue;
    transform: translateX(-110%);
    animation: slide-right 2s ease-in-out forwards;
    animation-delay: .8s;
}
</style>
