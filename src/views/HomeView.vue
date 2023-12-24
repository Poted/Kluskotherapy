<template>
  <div class="container">

    <header>
    <h1>Usługi Fizjoterapeutyczne</h1>
  </header>


    <section>
    <h2>1. Indywidualne Podejście</h2>
    <p>Każdy pacjent jest dla nas wyjątkowy. Przystępujemy do każdego przypadku z pełnym zaangażowaniem, starając się zrozumieć Twoje indywidualne potrzeby i cele zdrowotne.</p>

    <h2>2. Doświadczenie i Profesjonalizm</h2>
    <p>Nasi fizjoterapeuci posiadają bogate doświadczenie w obszarze rehabilitacji i terapii. Dzięki ich wiedzy oraz ciągłemu doskonaleniu umiejętności, możesz być pewien/pewna, że otrzymasz najwyższą jakość usług.</p>

    <h2>3. Nowoczesne Metody Leczenia</h2>
    <p>Stosujemy nowoczesne metody fizjoterapeutyczne, wykorzystując najnowsze osiągnięcia nauki. Naszym celem jest skuteczne leczenie oraz przyspieszenie procesu regeneracji.</p>

    <h2>4. Komfortowa Przestrzeń</h2>
    <p>Nasza przyjazna atmosfera i nowoczesne sale zabiegowe stwarzają komfortowe warunki do skoncentrowanej pracy nad Twoim zdrowiem.</p>

    <h2>5. Elastyczne Godziny Pracy</h2>
    <p>Zależy nam na Twojej wygodzie, dlatego oferujemy elastyczne godziny pracy, abyś mógł/mogła łatwo dostosować swoje wizyty do własnego harmonogramu.</p>
  </section>

  <div id="contact">
    <Contact />
  </div>


  </div>
</template>

<script setup>
import Contact from '@/components/Contact.vue'

</script>


<style lang="scss">
body {
  font-family: 'Open Sans', sans-serif;
  margin: 0;
  padding: 0;

  .container {
    display: flex;
    flex-direction: column;
    align-items: center;



  }

}
</style>