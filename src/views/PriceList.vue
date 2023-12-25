<template>
  <div class="container">

    <!-- <div class="header-text">
      <h1>Oferta</h1>
    </div> -->


    <section>
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

  </div>

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
.container {
  display: flex;
  flex-direction: column;
  align-items: center;

  .header-text {
    margin-top: 50px;
    text-align: center;
  }

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


  #contact {
    width: 80%;

    @media only screen and (max-width: 600px) {
      width: 95%;
    }
  }

  button {
    border: none;
    outline: none;
    padding: 10px 20px;
    border-radius: 50px;
    color: #333;
    background: #fff;
    box-shadow: 0 3px 20px 0 #0000003b;
    margin-top: 20px;
}

button:hover {
    cursor: pointer;
}


}
</style>