<template>
    <div class="flex justify-center py-5 items-center text-white bg-black">
            <router-link class="px-5" to="/">Home</router-link>
            <router-link class="px-5" to="/cartoons">Cartoons</router-link>
            <router-link class="px-5" to="/about">About</router-link>
    </div>
</template>


<script>
export default{
    components:'Navbar'
}
</script>