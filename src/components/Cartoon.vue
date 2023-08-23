<template>
  <div class="card card-compact w-96 h-auto mx-5 my-8  bg-base-100 shadow-xl">
    <figure>
      <img src="../images/minions.jpg" alt="Cartoon's İmage"/>
    </figure>
    <div class="card-body">
      <h2 class="card-title">{{ cart.title }}</h2>
      <p>{{ cart.description }}</p>
      <buttons class="btn btn-secondary">Beğendim</buttons>
    </div>

  </div>
</template>

<script>
import Cartoon from './Cartoon.vue';
import Buttons from './Buttons.vue';

export default {
  components: { Buttons },
  components: [
    Cartoon,
    Buttons,
  ],
  props: ['cart']
};
</script>Buttons