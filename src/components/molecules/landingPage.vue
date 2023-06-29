<template>
    <div id="landingPage">
        <div class="overlay">
            <h1 class="subtitle">LeadMark Landing Page</h1>
            <h1 class="title">We Are Creative</h1>  
        </div>  
        <div class="shape">
            <svg viewBox="0 0 1500 200">
                <path d="m 0,240 h 1500.4828 v -71.92164 c 0,0 -286.2763,-81.79324 -743.19024,-81.79324 C 300.37862,86.28512 0,168.07836 0,168.07836 Z"></path>
            </svg>
        </div>  
        <div class="mouse-icon"><div class="wheel"></div></div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    name:'landingPage'
})
</script>

<style scoped>
#landingPage {
    position: relative;
    height: 100vh;
    min-height: 500px;
    background: url(../../assets/header.jpg) no-repeat center center fixed;
    background-size: cover;
    overflow: hidden;
    display: block;
}

#landingPage .overlay {
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.7);
    color: #fff;
    display: flex;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    flex-direction: column;
    -webkit-box-pack: center;
    justify-content: center;
}
#landingPage .overlay .subtitle {
    font-size: calc(13px + (18 - 13) * ((100vw - 320px) / (1200 - 320)));
    font-weight: 400;
    margin-bottom: 0;
    letter-spacing: 8px;
    word-spacing: 10px;
    text-align: center;
    opacity: .8;

}
#landingPage .overlay .title {
    font-size: calc(30px + (70 - 30) * ((100vw - 320px) / (1200 - 320)));
    font-weight: bold;
}
#landingPage .shape svg {
    bottom: 0;
    position: absolute;
    left: 0;
    width: 100%;
    z-index: 9;
    overflow: hidden;
    vertical-align: middle;
}
#landingPage .shape svg path {
    fill: #fff;
}

.mouse-icon {
    border: 2px solid #fff;
    border-radius: 16px;
    height: 40px;
    width: 24px;
    display: block;
    z-index: 10;
    position: absolute;
    left: 0;
    right: 0;
    bottom: 100px;
    margin: auto;
}

.mouse-icon .wheel {
    position: relative;
    border-radius: 10px;
    background: #fff;
    width: 2px;
    height: 6px;
    top: 4px;
    margin-left: auto;
    margin-right: auto;
    animation-name: drop;
    animation-duration: 1.4s;
    animation-timing-function: linear;
    animation-delay: 0s;
    animation-iteration-count: infinite;
    animation-play-state: running;
}


@keyframes drop {
  0% {transform:  scaleY(1); opacity: 1;}
  50% {transform: translateY(20px) scaleY(1); opacity: 1;}
  100% {transform:  scaleY(0.9); opacity: 0;}
}

div {
    display: block;
}

</style>