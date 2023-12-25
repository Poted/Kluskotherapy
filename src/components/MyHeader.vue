<template>
    <header>
      <div class="overlay">
        <h1>Kluskotherapy</h1>
        <h2>Zaufaj profesjonalizmowi w trosce o Twoje zdrowie!</h2>     
        <button @click="readMore">Skontakuj się z nami</button>
        <div class="icons">
          <a href="https://www.facebook.com" target="_blank">
            <img src="../../public/fb.ico" alt="fb">
          </a>
          <a href="https://www.instagram.com" target="_blank">
            <img src="../../public/insta.ico" alt="insta">
          </a>
        </div>
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
    background: url('../../public/background.jpeg');
    text-align: center;
    width: 100%;
    height: auto;
    background-size: cover;
    background-attachment: fixed;
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
  
  header .overlay {
    display: flex;
    flex-direction: column;
    align-items: center;

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
  