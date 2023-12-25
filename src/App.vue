<template>
  <div class="container">

    <MyHeader />

    <RouterView />
    
    <MyFooter />

  </div>
</template>

<script setup>

import { RouterLink, RouterView } from 'vue-router'
import MyHeader from './components/MyHeader.vue'
import MyFooter from './components/MyFooter.vue'




</script>


<style lang="scss">

body {
  font-family: 'Open Sans', sans-serif;
  margin: 0;
  padding: 0;
}




</style>











    <!-- <header>
      <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header> -->