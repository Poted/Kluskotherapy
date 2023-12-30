<template>
  <!-- <div class="container"> -->

    <div class="header-text">
      <h1>Usługi Fizjoterapeutyczne</h1>
    </div>


    <section class="content">
      <div class="box">
        <div class="upper">
          <h2>1. Indywidualne Podejście</h2>
        </div>
        <div class="bottom">
          <p>Każdy pacjent jest dla nas wyjątkowy. Przystępujemy do każdego przypadku z pełnym zaangażowaniem, starając
            się
            zrozumieć Twoje indywidualne potrzeby i cele zdrowotne.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>2. Doświadczenie i Profesjonalizm</h2>
        </div>
        <div class="bottom">
          <p>Nasi fizjoterapeuci posiadają bogate doświadczenie w obszarze rehabilitacji i terapii. Dzięki ich wiedzy oraz
            ciągłemu doskonaleniu umiejętności, możesz być pewien/pewna, że otrzymasz najwyższą jakość usług.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>3. Nowoczesne Metody Leczenia</h2>
        </div>
        <div class="bottom">
          <p>Stosujemy nowoczesne metody fizjoterapeutyczne, wykorzystując najnowsze osiągnięcia nauki. Naszym celem jest
            skuteczne leczenie oraz przyspieszenie procesu regeneracji.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>4. Komfortowa Przestrzeń</h2>
        </div>
        <div class="bottom">
          <p>Nasza przyjazna atmosfera i nowoczesne sale zabiegowe stwarzają komfortowe warunki do skoncentrowanej pracy
            nad
            Twoim zdrowiem.</p>
        </div>
        <div class="image">
          <ImageWrap />
        </div>
      </div>

    </section>

    <div id="contact">
      <Contact />
    </div>


  <!-- </div> -->
</template>

<script setup>
import Contact from '@/components/Contact.vue'
import ImageWrap from '@/components/ImageWrap.vue'

</script>


<style lang="scss">

#contact {
    width: 80%;

    @media only screen and (max-width: 600px) {
      width: 95%;
    }
  }

// .container {
//   display: flex;
//   flex-direction: column;
//   align-items: center;

//   .header-text {
//     margin-top: 50px;
//     text-align: center;
//   }

//   .box {
//     border: 1px solid black;
//     border-radius: 10px;
//     margin: 50px;
//     box-shadow: 0px 0px 30px 2px #b1b1b1b2;
//     background-color: #f1f1f1;


//     .upper {
//       padding: 5px 20px 5px 20px;
//       background-color: #333;
//       background-image: linear-gradient(80deg, #52e3593f 10%, #38456757 100%);
//       border-top-left-radius: 10px;
//       border-top-right-radius: 10px;

//     }

//     .bottom {
//       padding: 8px 40px 8px 40px;
//     }

//     h2 {
//       color: white;
//     }

//     .image {
//       align-self: center;
//       margin-bottom: 20px;
//       display: flex;
//       flex-direction: column;
//       align-items: center;
//     }

//     display: flex;
//     flex-direction: column;

//     @media only screen and (max-width: 600px) {

//       margin: 30px 15px 30px 15px;

//       .upper {
//         padding: 8px 25px 8px 25px;
//         font-size: small;
//       }

//       .bottom {
//         padding: 5px 20px 5px 20px;
//       }

//       .image {
//         width: 80%;
//       }

//     }
//   }


//   #contact {
//     width: 80%;

//     @media only screen and (max-width: 600px) {
//       width: 95%;
//     }
//   }


// }

</style>