<template>
<div>
    <Header class="navbar">
        <div class="logo"><a href="#"><img src="../img/jksite.png" alt="" width="250px"></a></div>
        
        <div id="menuToggle">

    <input type="checkbox" />

    <span></span>
    <span></span>
    <span></span>

    <ul id="menu">
      <div class="logo-black"><a href="#"><img src="../img/jksite1.png" alt="" width="250px"></a></div>
      <div class="menu-main-info">
      <h1><a href="http://jksite.ru/"><li>My Site</li></a></h1>
      <h1><a href="https://account.rabota.ua/jobsearch/cvbuilder?resumeId=20844899"><li>About me</li></a></h1>
      <h1><a href="https://github.com/over284?tab=repositories"><li>My works</li></a></h1>
      </div>
      <div class="menu-second-info">
      <a href="https://t.me/Vad3x" target="_blank"><li>Telegram</li></a>
      <!-- <a href="https://discord.gg/gJ482Y2B2x" target="_blank"><li>Discord</li></a> -->
      <a href="https://instagram.com/vadim_st_vadim/" target="_blank"><li>Instagram</li></a>
      <a href="https://github.com/over284" target="_blank"><li>GitHub</li></a>
      </div>
    </ul>
  </div>

    </Header>
</div>
</template>

<style>
.logo-black{
  padding-right: 100px;
  margin: 24px 0px 0px 0px;
  cursor: pointer;
}

#menuToggle
{
  display: block;
  position: fixed;
  top: 60px;
  left: 95%;
  padding: 20px 10px 5px 10px;
  z-index: 1;
  -webkit-user-select: none;
  user-select: none;
  background: #000;
  border-radius: 50%;
}

#menuToggle input
{
  display: block;
  width: 50px;
  height: 50px;
  position: absolute;
  top: -2px;
  left: -8px;
  cursor: pointer;
  
  opacity: 0; /* hide this */
  z-index: 2; /* and place it over the hamburger */
  
  -webkit-touch-callout: none;
}

/*
 * Just a quick hamburger
 */
#menuToggle span
{
  display: block;
  width: 33px;
  height: 4px;
  margin-bottom: 5px;
  position: relative;
  background: rgb(255, 255, 255);
  border-radius: 3px;
  top: -5px;
  z-index: 1;
  
  transform-origin: 4px 0px;
  
  transition: transform 0.5s cubic-bezier(0.77,0.2,0.05,1.0),
              background 0.5s cubic-bezier(0.77,0.2,0.05,1.0),
              opacity 0.55s ease;
}

#menuToggle span:first-child
{
  transform-origin: 0% 0%;
}

#menuToggle span:nth-last-child(2)
{
  transform-origin: 0% 100%;
}

/* 
 * Transform all the slices of hamburger
 * into a crossmark.
 */
#menuToggle input:checked ~ span
{
  opacity: 1;
  transform: rotate(45deg) translate(-2px, -1px);
  background: #232323;
}

/*
 * But let's hide the middle one.
 */
#menuToggle input:checked ~ span:nth-last-child(3)
{
  opacity: 0;
  transform: rotate(0deg) scale(0.2, 0.2);
}

/*
 * Ohyeah and the last one should go the other direction
 */
#menuToggle input:checked ~ span:nth-last-child(2)
{
  transform: rotate(-45deg) translate(0, -1px);
}

/*
 * Make this absolute positioned
 * at the top left of the screen
 */
#menu
{
  position: absolute;
  width: 350px;
  height: 100vh;
  margin: -140px 0 0 510px;
  padding: 60px 0px 0px 20px;
  
  background: #ffffff;
  list-style-type: none;
  -webkit-font-smoothing: antialiased;
  /* to stop flickering of text in safari */
  
  transform-origin: 0% 0%;
  transform: translate(-100%, 0);
  
  transition: transform 0.5s cubic-bezier(0.77,0.2,0.05,1.0);
}
.menu-main-info{
  padding-top: 50px;
  padding-bottom: 30px;
  font-size: 14px;
  padding-right: 180px;
}
.menu-second-info{
  font-size: 24px;
  padding-right: 180px;
}
#menu li
{
  padding: 10px 0px 0px 20px;
  
}
#menu a:hover{
  color: rgb(255, 0, 0);
  transition: .2s;
}
#menu a{
  text-decoration: none;
  color: #000;
}

/*
 * And let's slide it in from the left
 */
#menuToggle input:checked ~ ul
{
  transform: translate(-800px);
}

.navbar {
  
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 50px 0px 0px 0px;
    display: flex;
    justify-content: space-between;
    color: aliceblue;
    align-items: center;
    z-index: 999;
}
.logo {
    margin: 0px 0px 0px 50px;
    cursor: pointer;
}
</style>
<script>
</script>