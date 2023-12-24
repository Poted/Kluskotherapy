<template>
    <header>
      <div class="overlay">
        <h1>Kluskotherapy</h1>
        <h2>Zaufaj profesjonalizmowi w trosce o Twoje zdrowie!</h2>
        <!-- <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Vero nostrum quis, odio veniam itaque ullam debitis
          qui magnam consequatur ab. Vero nostrum quis, odio veniam itaque ullam debitis qui magnam consequatur ab.
        </p> -->
        <br />
        <button @click="readMore">Skontakuj się z nami</button>
      </div>
    </header>
  </template>
  
  <script setup>

    const readMore = () => {

      const section = document.getElementById('contact');
      section.scrollIntoView({ behavior: 'smooth' });

    };

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
    background: url('https://images.pexels.com/photos/2382325/pexels-photo-2382325.jpeg');
    text-align: center;
    width: 100%;
    height: auto;
    background-size: cover;
    background-attachment: fixed;
    position: relative;
    overflow: hidden;
    border-radius: 0 0 85% 85% / 30%;
  }
  
  header .overlay {
    width: 100%;
    height: 100%;
    padding: 50px;
    color: #fff;
    text-shadow: 4px 6px 3px #333;
    background-image: linear-gradient(80deg, #52e3593f 10%, #38456757 100%);
  }
  
  h1 {
    font-size: 10vw;
    margin-bottom: 30px;


  }
  
  h2,
  p {
    font-family: 'Open Sans', sans-serif;
    margin-bottom: 30px;
  }
  
  button {
    border: none;
    outline: none;
    padding: 10px 20px;
    border-radius: 50px;
    color: #333;
    background: #fff;
    margin-bottom: 50px;
    box-shadow: 0 3px 20px 0 #0000003b;
  }
  
  button:hover {
    cursor: pointer;
  }
  </style>
  