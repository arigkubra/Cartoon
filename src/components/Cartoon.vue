<template>
  <div class="card card-compact w-96 h-96 mx-5 my-28 bg-base-100 shadow-xl">
    <figure>
      <img :src="cart.img" alt="Cartoon's İmage"/>
    </figure>
    <div class="card-body">
      <h2 class="card-title">{{ cart.title }}</h2>
      <p>{{ cart.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  components: "Cartoon",
  props: ['cart']
};
</script>