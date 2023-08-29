<template>
  <div class="relative  bg-black">
    <img class="w-screen h-screen object-cover " src="../images/kobby-mendez-d0oYF8hm4GI-unsplash.jpg" alt="background image">
    <div class="absolute left-5 md:right-96 top-32 md:top-40  text-white text-3xl md:text-6xl">Welcome to</div>
    <div class="absolute left-10 md:right-12 top-44 md:top-60  text-white text-3xl md:text-6xl">The World of Cartoon</div>
    <button class="absolute left-56 md:right-80 top-56 md:top-80 rounded-lg w-28 md:w-48 btn-lg  bg-gradient-to-r from-cyan-500 to-blue-500 text-white">
      <router-link to="/cartoons">Cartoons</router-link> 
    </button>
  </div>
</template>

<script>
import Buttons from '@/components/Buttons.vue';

export default {
  name: 'HomeView',
  components: {
    Buttons,
  }
}
</script>
