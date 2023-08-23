<template >
  <div
    class="flex  justify-center items-center bg-gradient-to-b from-black to-grey ">
    <Cartoon v-for="cart in cartoonItems" :key="cart.title" :cart="cart" />
    

  </div>
</template>

<script>
import Cartoon from "@/components/Cartoon.vue";
export default {
  data(){
    return{
      cartoonItems:[
        { title:'Minions', img:'../images/minions.jpg' ,description: 'Minions is a 2015 American computer-animated comedy film directed by Pierre Coffin and Kyle Balda, produced by Chris Meledandri and Janet Healy, and written by Brian Lynch. Produced by Illumination Entertainment and distributed by Universal Pictures, it is the spin-off/prequel[a] to Despicable Me (2010). ' },
        { title:'Minnie Mouse', img:'../images/minnimouse.jpg' ,description:'Minnie Mouse is a cartoon character created by The Walt Disney Company. As the longtime sweetheart of Mickey Mouse, she is an anthropomorphic mouse with white gloves, a red or pink bow, blue polka-dotted dress, white bloomers and low-heeled shoes occasionally with ribbons on them.'  },
        { title:'Toy Story', img:'../images/toystory.jpg' ,description:'Toy Story is a 1995 American computer-animated comedy film produced by Pixar Animation Studios and released by Walt Disney Pictures. The first installment in the Toy Story franchise, it was the first entirely computer-animated feature film, as well as the first feature film from Pixar.' }
      ]
    }
  },
  components: {
    Cartoon,
    
  },
};
</script>