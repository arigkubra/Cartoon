<template>
  <div class="bg-gradient-to-b from-black to-grey">
    <h1 class="text-6xl flex justify-center items-center py-11 text-white">About Us</h1>

    <div class="overflow-x-auto mx-16 pt-6 pb-24">
      <table class="table">
        <!-- head -->
        <thead>
          <tr>
            <th>Name</th>
            <th>Job</th>
            <th></th>
          </tr>
        </thead>
        <tbody>
          <Row />
          <Row />
          <Row />
          <Row />
        </tbody>
        
      </table>
    </div>
  </div>
</template>
<script>
import Row from '@/components/Row.vue';
export default{
  components:{
    Row,
  }
}
</script>
