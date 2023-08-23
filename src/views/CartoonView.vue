<template >
  <div
    class="flex flex-wrap pt-12 justify-center items-center bg-gradient-to-b from-black to-grey h-screen w-screen">
    <Cartoon />
    <Cartoon />
    <Cartoon />
    
  </div>
</template>

<script>
import Cartoon from "@/components/Cartoon.vue";

export default {
  components: {
    Cartoon,
  },
};
</script>