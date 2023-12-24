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

.container {
  background-color: white;

  // background-image: linear-gradient(80deg,  10%, #39832757 100%);
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