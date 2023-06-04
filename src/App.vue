

<template>
 
  <div>
    <Header />
    <banner />
    <ctag />
  </div>
  
</template>
<script setup>
// import { RouterLink, RouterView } from 'vue-router'
import Header from  './components/header.vue'
import banner from './components/banner.vue'
import ctag from './components/catagorie.vue'

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
  .container{
      max-width: calc(1440px - 170px);
        width: 100%;
        margin: auto;
  }
</style>
