<template>
    <div class="map-outer">
      <div class="gmap-canvas">
        <iframe
          :src="mapSrc"
          frameborder="0"
          scrolling="no"
          style="width: 100%; height: 400px;"
        ></iframe>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        mapSrc: 'https://maps.google.com/maps?q=trudna%20bochnia%2022&t=&z=17&ie=UTF8&iwloc=&output=embed',
      };
    },
  };
  </script>
  
  <style scoped>
  .map-outer {
    position: relative;
    /* height: 400px; */
    width: 100%;
    background: #fff;
    text-align: center;
    box-shadow: 0px 0px 50px 5px #E8E8E8;
    margin: 50px 0 30px 0;
  }
  
  .gmap-canvas {
    overflow: hidden;
    height: 400px;
  }
  
  .gmap-canvas iframe {
    position: relative;
    z-index: 2;
  }
  
  .map-link {
    color: #fff !important;
    position: absolute !important;
    top: 0 !important;
    z-index: 0 !important;
  }
  </style>
  