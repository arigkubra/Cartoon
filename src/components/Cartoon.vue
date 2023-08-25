<template>
  <div class="card card-compact w-96 h-auto mx-5 my-8  bg-base-100 shadow-xl">
    
    <figure>
      <img src="../images/minions.jpg" alt="Cartoon's İmage"/>
    </figure>
    <div v-if="isFav" class="rating gap-1 flex justify-center items-center flex-col mt-12">
      <p>Added to Favorites</p>
      <input type="radio" name="rating-3" class="mask mask-heart bg-violet-500" />
    </div>
    <div class="card-body">
      <h2 class="card-title my-2">{{ cart.title }}</h2>
      <p class="my-3">{{ cart.description }}</p>
      

      <buttons class="btn btn-secondary" @click="addFav">Add to favorites</buttons>
      <buttons v-if="isFav"  @click="delFav" class="btn btn-error">Delete the favorites</buttons>
    </div>

  </div>
</template>

<script>
import Cartoon from './Cartoon.vue';
import Buttons from './Buttons.vue';

export default {
  data(){
    return{
      isFav: false
    }
  },
  methods:{
    addFav (){
      this.isFav = true
    },
    delFav(){
      this.isFav = false
    }
  },
  components: [
    Cartoon,
    Buttons,
  ],
  props: ['cart']
};
</script>