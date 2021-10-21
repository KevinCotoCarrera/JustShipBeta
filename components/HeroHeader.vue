<template>
<div id="header" class="flex flex-col text-center justify-center text-white">
        <div class="flex justify-between">
            <img src="../assets/black.svg" class=" mt-5 ml-3 w-14 h-14 sm:w-20 sm:h-20 xl:w-28 xl:h-28"/>
            
        </div>
       
        <div class="flex flex-col justify-center text-center items-center mt-8 ml-3 mr-3">
        <h1 class="text-2xl sm:text-3xl xl:text-5xl font-semibold w-40 xl:w-60 sm:-ml-36 sm:text-center">Solo Lanza</h1>
        <p class="text-base sm:text-lg xl:text-2xl sm:text-left  font-normal mt-5 sm:mt-8 xl:mt-12 mb-5 sm:mb-8 xl:mb-12 w-3/4 sm:w-96 sm:-ml-36">Lancemos tu producto hoy, convierte con nosotros tus dudas en combustible, suscríbete ahora para obtener beneficios.</p>
        <a href="#form-section"><button  class="flex justify-center  items-center content-center  sm:-ml-36 mr-1 text-base sm:text-lg xl:text-2xl bg-white px-4 sm:px-6 xl:px-16 w-24 sm:w-28 xl-36 h-8 sm:h-10 xl:h-14 rounded-lg sm:rounded-xl shadow-sm sm:shadow-md mb-3 sm:mb-5 xl:mb-8 " id="btn-sub">Suscribete</button></a> 
       <a href="#donate-section">  <button  class="tex-base sm:text-lg xl:text-2xl  bg-transparent sm:-ml-36 w-24 sm:w-28 xl:w-36 h-8 sm:h-10">Dona</button> </a> 
       <img class=" w-40 sm:w-60 h-40 sm:h-60 xl:w-72 xl:h-72 2xl:w-80 2xl:h-80 mt-4 sm:absolute sm:right-4 xl:right-20 sm:-mt-20"  src="../assets/launching-pana.svg"/>
        
        </div>
       
        
        <svg class="waves" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
        viewBox="0 24 150 28" preserveAspectRatio="none" shape-rendering="auto">
        <defs>
        <path id="gentle-wave" d="M-160 44c30 0 58-18 88-18s 58 18 88 18 58-18 88-18 58 18 88 18 v44h-352z" />
        </defs>
        <g class="parallax">
        <use xlink:href="#gentle-wave" x="48" y="0" fill="rgba(255,255,255,0.7" />
        <use xlink:href="#gentle-wave" x="48" y="3" fill="rgba(255,255,255,0.5)" />
        <use xlink:href="#gentle-wave" x="48" y="5" fill="rgba(255,255,255,0.3)" />
        <use xlink:href="#gentle-wave" x="48" y="7" fill="#fff" />
</g>
</svg>

</div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
#header{
    background: linear-gradient(60deg, #ee8f5f 0%, #f8d257 100%);
    color: #333;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;

}
#btn-sub{
    color:#ee8f5f
}
.waves {
  position:relative;
  width: 100%;
  height:15vh;
  margin-bottom:-7px; /*Fix for safari gap*/
  min-height:100px;
  max-height:150px;}



/* Animation */

.parallax > use {
  animation: move-forever 25s cubic-bezier(.55,.5,.45,.5)     infinite;
}
.parallax > use:nth-child(1) {
  animation-delay: -2s;
  animation-duration: 7s;
}
.parallax > use:nth-child(2) {
  animation-delay: -3s;
  animation-duration: 10s;
}
.parallax > use:nth-child(3) {
  animation-delay: -4s;
  animation-duration: 13s;
}
.parallax > use:nth-child(4) {
  animation-delay: -5s;
  animation-duration: 20s;
}
@keyframes move-forever {
  0% {
   transform: translate3d(-90px,0,0);
  }
  100% { 
    transform: translate3d(85px,0,0);
  }
}
/*Shrinking for mobile*/
@media (max-width: 768px) {
  .waves {
    height:40px;
    min-height:40px;
  }}
</style>
