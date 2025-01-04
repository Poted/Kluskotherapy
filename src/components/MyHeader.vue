<template>
  <header>

    <div class="overlay">

      <h1>FizjoStacja</h1>
      <h2>mgr Julia Poprawa</h2>

      <h3>Aktualności i promocje na</h3>
      <br>
    
      <div class="icons">
    
        <a href="https://www.facebook.com/people/FizjoStacja-Julia-Poprawa/61554824174356/" target="_blank">
          <img src="/fb.ico" alt="fb"> 
        </a>
    
        <a href="https://l.messenger.com/l.php?u=https%3A%2F%2Fwww.instagram.com%2Ffizjostacja.bochnia%3Figsh%3DMXJ1MDV3ZmE1ZjUwZg%253D%253D&h=AT3rAMM10MzxSzdONGEsBtlBD_L008B0IE35yvuBBj4YXos7LwGINsshJErIsjDD_b3f3QSFTo_-tq7I74VS2hMVPYzPCtV5qvy-q48AdDHbU6hAAVR0u9RKy7KUBFs9GhDQ6g" target="_blank">
          <img src="/insta.ico" alt="insta">
        </a>
    
      </div>
    
    </div>

  </header>
</template>
  
<script setup>

</script>
  
<style scoped lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  height: 900px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

header {
  background: url('../../public/background.webp');
  text-align: center;
  width: 100%;
  height: auto;
  background-size: cover;
  position: relative;
  overflow: hidden;
  border-radius: 0 0 85% 85% / 30%;
}

.icons {

  img {
    width: 50px;
    margin: -30px 30px -20px 30px;
  }
}

button {
  width: 100px;
  background-color: red;
  height: 100px;
}


header .overlay {
  display: flex;
  flex-direction: column;

  width: 100%;
  height: 100%;
  padding: 50px;
  color: #fff;
  text-shadow: 4px 6px 3px #333;
  background-image: linear-gradient(80deg, #52e3593f 10%, #38456757 100%);
}


h1, h2 {
  font-family: "Great Vibes", cursive;
  font-weight: 600;
  font-style: normal;
}


h1 {
  font-size: 12vw;

  @media only screen and (max-width: 600px) {
    font-size: 18vw;
    align-self: center;
    max-width: 100vw;
  }
}

h2 {
  font-size: 5vw;

  @media only screen and (max-width: 600px) {
    font-size: 9vw;
    align-self: center;
    max-width: 100vw;
  }
}

</style>
  