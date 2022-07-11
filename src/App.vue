<template>
<div id="app">
    <Preloader />
    <Header />
    <First />
    <Second />
    <Third />
    <Fourth />
    <Five />
    <Footer/>
    
</div>
</template>

<script>
import Preloader from './components/mainPreloader.vue'
import Header from './components/mainHeader.vue'
import First from './components/firstSection.vue'
import Second from './components/secondSection.vue'
import Third from './components/thirdSection.vue'
import Fourth from './components/fourthSection.vue'
import Five from './components/fiveSection.vue'
import Footer from './components/mainFooter.vue'


export default {
    components: {
        Preloader,
        Header,
        First,
        Second,
        Third,
        Fourth,
        Five,
        Footer
    },
}
</script>

<style>
@font-face {
    font-family: '1';
    font-display: block;
    src: url('./fonts/Joan-Regular.ttf');
}

@font-face {
    font-family: '2';
    font-display: block;
    src: url('./fonts/MeriendaOne-Regular.ttf');
}

body::-webkit-scrollbar {
    width: 8px;
}

body::-webkit-scrollbar-track {
    box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);

}

body::-webkit-scrollbar-thumb {
    background-color: #fd0202;
    outline: 1px solid slategrey;
}

body {
    width: 100%;
    overflow-x: hidden;
    margin: 0;
    padding: 0;
    font-family: '1';
    background: #000;
    color: aliceblue;
}

h1 {
    margin: 0;
}
</style>
