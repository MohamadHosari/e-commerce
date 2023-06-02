

<template>
 
  <div>
    <Header />
    <banner />
  </div>
  
</template>
<script setup>
// import { RouterLink, RouterView } from 'vue-router'
import Header from  './components/header.vue'
import banner from './components/banner.vue'

</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@300&display=swap');

  *{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Nunito Sans', sans-serif;
}
body{
  color: #121212;
}
</style>
