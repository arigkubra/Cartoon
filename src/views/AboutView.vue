<template>
  <div class="bg-gradient-to-b from-black to-grey">
    <h1 class="text-6xl flex justify-center items-center py-11 text-white">About Us</h1>

    <div class="overflow-x-auto mx-16 pt-6 pb-24">
      <table class="table">
        <!-- head -->
        <thead class="text-white">
          <tr>
            <th>Name</th>
            <th>Job</th>
            <th></th>
          </tr>
        </thead>
        <tbody>
          <Row v-for="person in people" :key="person.fname" :person="person" />
        </tbody>
        
      </table>
    </div>
  </div>
</template>
<script>
import Row from '@/components/Row.vue';
export default{
  data(){
    return{
      people:[
        {fname:'Kübra A.', company:'GitLab', job:'Front End Developer' },
        {fname:'Teslime M.', company:'Apple', job:'Back End Developer' },
        {fname:'Kübra T.', company:'Microsoft', job:'Full Stack Developer' },
        {fname:'Merve B.', company:'Huawei', job:'Front End Developer' },
      ]
    }
  },
  components:{
    Row,
  }
}
</script>
