<template>
  <!-- <div class="container"> -->

    <!-- <div class="header-text">
      <h1>Oferta</h1>
    </div> -->


    <section class="content">
      <div class="box">
        <div class="upper">
          <h2>1. Indywidualna Ocena Stanu Zdrowia</h2>
        </div>
        <div class="bottom">
          <p>• Pełna ocena fizjoterapeutyczna.</p>
          <p>• Analiza historii medycznej pacjenta.</p>
          <p>• Badanie fizyczne i funkcjonalne.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>2. Terapia Manualna</h2>
        </div>
        <div class="bottom">
          <p>• Manipulacje stawów i tkanek miękkich.</p>
          <p>• Techniki mobilizacji.</p>
          <p>• Terapia masażem.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>3. Ćwiczenia Terapeutyczne</h2>
        </div>
        <div class="bottom">
          <p>• Opracowanie spersonalizowanego programu ćwiczeń.</p>
          <p>• Ćwiczenia wzmacniające i stabilizujące.</p>
          <p>• Programy rehabilitacyjne.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>4. Terapia Urazy i Zwichnięcia</h2>
        </div>
        <div class="bottom">
          <p>• Rehabilitacja po urazach sportowych.</p>
          <p>• Terapia po operacjach ortopedycznych.</p>
          <p>• Leczenie zwichnięć i naderwań.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>5. Fizykoterapia</h2>
        </div>
        <div class="bottom">
          <p>• Elektroterapia.</p>
          <p>• Ultradźwięki.</p>
          <p>• Krioterapia i termoterapia.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>6. Terapia Nerwów i Mięśni</h2>
        </div>
        <div class="bottom">
          <p>• Leczenie bólów nerwobólowych.</p>
          <p>• Terapia mięśniowo-powięziowa.</p>
          <p>• Ćwiczenia na poprawę koordynacji.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>7. Porady dotyczące Ergonomii i Postawy</h2>
        </div>
        <div class="bottom">
          <p>• Ocena postawy ciała.</p>
          <p>• Szkolenie z ergonomii w miejscu pracy.</p>
          <p>• Porady dotyczące poprawy postawy.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>8. Terapia dla Grup Specjalnych</h2>
        </div>
        <div class="bottom">
          <p>• Fizjoterapia dzieci i niemowląt.</p>
          <p>• Opieka nad pacjentami geriatrycznymi.</p>
          <p>• Terapia w przypadku schorzeń neurologicznych.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>9. Konsultacje Online i Telemedycyna</h2>
        </div>
        <div class="bottom">
          <p>• Konsultacje zdalne dla wygody pacjentów.</p>
          <p>• Przesyłanie planów ćwiczeń i porad online.</p>
        </div>
      </div>

      <div class="box">
        <div class="upper">
          <h2>10. Programy Profilaktyczne</h2>
        </div>
        <div class="bottom">
          <p>• Edukacja dotycząca zdrowego stylu życia.</p>
          <p>• Programy profilaktyczne dla różnych grup wiekowych.</p>
          <p>• Zapobieganie kontuzjom i bólom kręgosłupa.</p>
        </div>
      </div>
    </section>

  <!-- </div> -->

  <button @click="goTop">Wróć na górę</button>
</template>

<script setup>

const goTop = () => {
  window.scrollTo({
    top: 0,
    behavior: 'smooth',
  });
};

</script>


<style lang="scss">
</style>