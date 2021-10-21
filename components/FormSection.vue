<template >
    <div  class="flex flex-col justify-center content-center text-center items-center">
    <h2 class="text-2xl sm:text-3xl xl:text-5xl font-semibold -mt-5">¿Deseas saber acerca de nuestro progreso?</h2>
    <p class="text-base sm:text-lg xl:text-2xl sm:w-96 mt-2 font-normal mr-4 ml-4 text-center">Con gusto te dejaremos saber</p>
    <input class="text-xl sm:text-2xl xl:text-3xl   mt-10  w-56 sm:w-96 h-10 sm:h-12 xl:h-16 shadow-xl rounded-xl" v-model="message" placeholder="levelsio@gmail.com">
   
     <button @click="check" class="p-3 text-xl sm:text-2xl xl:text-3xl  flex justify-center  items-center content-center  bg-white px-6 sm:px-8 xl:px-20 w-28 sm:w-32 xl:w-40 h-10 sm:h-12 xl:h-14 rounded-lg sm:rounded-xl shadow-sm sm:shadow-md mb-20 mt-2" id="btn-sub">Suscríbete</button>
     <span id="emailOk" class="hidden bg-green-400 opacity-50 rounded-sm text-white p-2 mt-2 relative bottom-14">Suscrito con éxito</span>
    </div>
</template>
<script>
export default {
   methods: {
       check(){
         var emailOk = document.getElementById("emailOk")
         emailOk.classList.remove("hidden")  
       }
   }
}
</script>
<style scoped>
#btn-sub{
    color:#ee8f5f
}
</style>