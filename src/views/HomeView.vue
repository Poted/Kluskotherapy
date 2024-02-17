<template>
  <!-- <div class="container"> -->

    <div class="header-text">
      <h1>Usługi Fizjoterapeutyczne</h1>
    </div>


    <section class="content">
      <div class="box">
        <div class="upper">
          <h2>Terapia indywidualna</h2>
        </div>
        <div class="bottom">
          <p>Pierwsza wizyta to 45 minut terapii oraz około 15 minut na przeprowadzenie wywiadu i zapoznanie się z dokumentacją medyczną pacjenta.
            <br>
            <br> Uprzejmię proszę o zabranie ze sobą wygodnego stroju sportowego niekrępującego ruchów przy ewentualnych ćwiczeniach.
          </p>
          <p style="font-weight: bold;">Cena: 130zł</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>Kinesiotaping</h2>
        </div>
        <div class="bottom">
          <p style="font-weight: bold;">
            Cena: od 30zł (cena ustalana indywidualnie)
          </p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>Fizykoterapia</h2>
        </div>
        <div class="bottom">
          <p>
            • Ultradźwięki <br>
            • Fonoforeza <br>
            • Laseroterapia <br>
            • Elektroterapia 
          </p>
          <p style="font-weight: bold;">
            Cena: 12zł
          </p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>Masaż</h2>
        </div>
        <div class="bottom">
          <p>• 30 minut: <strong>60zł</strong></p>
          <p>• 40 minut: <strong>80zł</strong></p>
          <p>• 60 minut: <strong>120zł</strong></p>
          <p>• 90 minut: <strong>180zł</strong></p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>Ćwiczenia indywidualne</h2>
        </div>
        <div class="bottom">
          <p>• 20 minut: <strong>40zł</strong></p>
          <p>• 45 minut: <strong>80zł</strong></p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>Komfortowa Przestrzeń</h2>
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

</style>