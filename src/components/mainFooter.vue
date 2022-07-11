<template>
<section class="footer-section-main">
    <div class="footer-section-info-left">
        <div class="info-links-left">
            <div class="link-description-left">Contact with me:</div>
            <div class="description-left-1">My Number: <br> +38 (050) 980-50-27 <br> 
            My Email: <br> vadst.28@gmail.com </div>
            <div class="footer-logo-left">
                <div class="logo-left"><a href="#"><img src="../img/jksite.png" alt="" width="600px"></a></div>
            </div>
        </div>
    </div>
    <div class="footer-section-info-right">
        <div class="info-links-right">
            <div class="link-description-right">Contact links:</div>
            <div class="link-box"><a href="https://github.com/over284">
                    <div class="link-icon"><img src="../icon/icons8-github.svg" alt="" width="66"></div>
                    <div class="link-name">GitHub</div>
                </a>
            </div>
            <div class="link-box"><a href="https://t.me/Vad3x">
                    <div class="link-icon"><img src="../icon/icons8-телеграмма-app.svg" alt="" width="66"></div>
                    <div class="link-name">Telegram</div>
                </a>
            </div>
            <div class="link-box"><a href="https://www.instagram.com/vadim_st_vadim/">
                    <div class="link-icon"><img src="../icon/icons8-instagram.svg" alt="" width="66"></div>
                    <div class="link-name">Instagram</div>
                </a>
            </div>
            <div class="link-description-right-2">You can also find me here:</div>
            <div class="link-box"><a href="https://vk.com/id32547665">
                    <div class="link-icon"><img src="../icon/icons8-vk-в-круге.svg" alt="" width="66"></div>
                    <div class="link-name">VKontakte</div>
                </a>
            </div>
            <div class="link-box"><a href="https://steamcommunity.com/profiles/76561198244486198/">
                    <div class="link-icon"><img src="../icon/icons8-steam.svg" alt="" width="66"></div>
                    <div class="link-name">Steam</div>
                </a>
            </div>
            <div class="link-box"><a href="https://discord.gg/gJ482Y2B2x">
                    <div class="link-icon"><img src="../icon/icons8-discord.svg" alt="" width="66"></div>
                    <div class="link-name">Discrord</div>
                </a>
            </div>
        </div>
    </div>
</section>
</template>

<style>
.footer-section-main {
    display: flex;
    height: 100vh;
    min-height: 700px;
}

.footer-section-info-left {
    width: 50%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    padding: 120px 40px 75px 6.6%;
}

.footer-section-info-right {
    width: 50%;
    background: #fff;
}

.info-links-right {
    display: flex;
    flex-direction: column;
}

.link-description-right {
    padding: 60px 0px 20px 100px;
    color: #000;
    font-size: 28px;
}
.link-description-right-2 {
    padding: 10px 0px 20px 100px;
    color: #000;
    font-size: 28px;
}

.link-box a {
    display: flex;
    margin-left: 100px;
    width: 0px;
    text-align: center;
    text-decoration: none;
}

.link-icon {}

.link-name {
    padding-left: 20px;
    color: #000;
    font-size: 24px;
    line-height: 65px;
}

.link-name:hover {
    color: rgb(255, 0, 0);
    transition: .2s;
}
.info-links-left {
    display: flex;
    flex-direction: column;
    height: 100%;
    padding-top: 40px;
    line-height: 32px;
}

.link-description-left {
    color: #fff;
    font-size: 28px;
}
.description-left-1 {
    padding-top: 20px;
    font-size: 24px;
    line-height: 42px;
}
.footer-logo-left {
    padding-top: 40px;
}
</style>
