<template class="container">

  
  <div class="menu">
    <button>Cennik: </button>
    <button v-if="currentPage === '/'" @click="readMore">↓ Kontakt ↓</button>
    <!-- <button v-if="currentPage === '/cennik'" style="margin-bottom: 40px;" @click="$router.push('/')">Wróć do strony głównej</button> -->
    <!-- <button v-if="currentPage === '/'" style="margin-bottom: 10px;" @click="$router.push('/cennik')">Sprawdź naszą ofertę</button>  -->
  </div>

    <section class="content">
      <div class="box">
        <div class="upper">
          <h2>Terapia indywidualna</h2>
        </div>
        <div class="bottom">
          <p><strong>• 45 minut:</strong> 170zł</p>
        </div>
      </div>
      
      <div class="box">
        <div class="upper">
          <h2>Konsultacja fizjoterapeutyczna</h2>
        </div>
        <div class="bottom">
          <p><strong>• do 20 minut:</strong> 50zł</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>Kinesiotaping</h2>
        </div>
        <div class="bottom">
          <p>
            <strong>
            Cena:
            </strong> od 40zł <strong>
            (cena ustalana indywidualnie)
            </strong>
          </p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>Fizykoterapia</h2>
        </div>
        <div class="bottom">
          <p>
            <strong>
            • Ultradźwięki <br>
            • Fonoforeza <br>
            • Laseroterapia <br>
            • Elektroterapia
            </strong> 
          </p>
          <p style="font-weight:400;">
            Cena: 20zł
          </p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>Masaż</h2>
        </div>
        <div class="bottom">
          <p><strong>• 30 minut:</strong> 90zł</p>
          <p><strong>• 40 minut:</strong> 120zł</p>
          <p><strong>• 60 minut:</strong> 160zł</p>
          <p><strong>• 90 minut:</strong> 220zł</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>Ćwiczenia indywidualne</h2>
        </div>
        <div class="bottom">
          <p><strong>• 20 minut:</strong> 60zł</p>
          <p><strong>• 45 minut:</strong> 100zł</p>
        </div>
      </div>

    </section>

    <div id="contact">
      <Contact />
    </div>

</template>

<script setup>
import Contact from '@/components/Contact.vue'

import { useRouter } from 'vue-router';
import { ref } from 'vue';

const router = useRouter()
const currentPage = ref('/');

const readMore = () => {

  const section = document.getElementById('contact');
  section.scrollIntoView({ behavior: 'smooth' });

};

router.afterEach((to) => {
  currentPage.value = to.path;
});


</script>

<style lang="scss">

.container {

  font-family: "M PLUS Rounded 1c", sans-serif;
  font-weight: 200;
  font-style: normal;

  h2 {
    margin: 2px 0px
  }

  .menu {

    display: flex;
    flex-direction: row;
    justify-content: space-around;
    width: 100%;
    
  button {
    
    font-family: "M PLUS Rounded 1c", sans-serif;
    font-weight: 900;
    font-style: normal;
  
    border: none;
    outline: none;
    padding: 10px 25px;
    border-radius: 15px;
    color: #333;
    background: #fff;
    box-shadow: 0 3px 20px 0 #0000003b;
    margin: 40px 0px 0px 0px;
  }

  button:hover {
    cursor: pointer;
  }
}


  
  @media only screen and (min-width: 1024px) {

    h2 {
      margin: 5px 0px
    }

    .menu {
      button {
        font-size: 2vh;
      }
    }
  }
}
</style>
