<template>
  <div class="container">

    <MyHeader />

    <!-- <img class="julia" src="../../public/julia.jfif" /> -->

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

  @media only screen and (max-width: 280px) {
    width: 104%;
  }
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;

  .julia {
    height: 60vh;
    position: fixed;

    left: 0;
    top: 10vh;
      
    z-index: -1;


  }

  .header-text {
    margin-top: 50px;
    text-align: center;
  }

  .content {

    width: 75%;

    .box {
      border: 1px solid black;
      border-radius: 10px;
      margin: 50px;
      box-shadow: 0px 0px 30px 2px #b1b1b1b2;
      background-color: #f1f1f1;


      .upper {
        padding: 5px 20px 5px 20px;
        background-color: #333;
        background-image: linear-gradient(80deg, #52e3593f 10%, #38456757 100%);
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;

      }

      .bottom {
        padding: 8px 40px 8px 40px;
      }

      h2 {
        color: white;
      }

      .image {
        align-self: center;
        margin-bottom: 20px;
        display: flex;
        flex-direction: column;
        align-items: center;
      }

      display: flex;
      flex-direction: column;

      @media only screen and (max-width: 600px) {

        margin: 30px 15px 30px 15px;

        .upper {
          padding: 8px 25px 8px 25px;
          font-size: small;
        }

        .bottom {
          padding: 5px 20px 5px 20px;
        }

        .image {
          width: 80%;
        }

      }

    }

    @media only screen and (max-width: 600px) {
      width: 95%;
    }

  }

}
</style>