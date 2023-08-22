<template>
  <div class="relative  bg-black">
    <img class="w-screen h-screen object-cover " src="../images/kobby-mendez-d0oYF8hm4GI-unsplash.jpg" alt="background image">
    <div class="absolute right-96 top-40  text-white text-6xl">Welcome to</div>
    <div class="absolute right-12 top-60  text-white text-6xl">The World of Cartoon</div>
    <button class="absolute right-80 top-80 rounded-lg btn-lg  bg-gradient-to-r from-cyan-500 to-blue-500 text-white"> <router-link class="" to="/cartoons">Cartoons</router-link> </button>
  </div>
</template>

<script>


export default {
  name: 'HomeView',
  components: {
    
  }
}
</script>
