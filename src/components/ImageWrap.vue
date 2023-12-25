<template>
    <div>
      <div id="wrap" class="img-wrap">
        <img
          src="https://scontent-waw1-1.xx.fbcdn.net/v/t1.15752-9/403394328_890183829072000_4380863316342879423_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=8cd0a2&_nc_ohc=HifIKnoIv30AX97I3aX&_nc_ht=scontent-waw1-1.xx&oh=03_AdRW8nM_e2UYA77Fhn9tqNK21-SLTmw_UnZgmaAn8xTqJg&oe=65B0DB88"
          width="360"
          height="360"
          alt=""
        />
      </div>
  
      <div class="controls">
        <div class="control">
          <label for="distance">Distance</label>
          <input
            type="range"
            max="100"
            v-model="distance"
            @input="updateDistance"
            title="Distance"
          />
        </div>
        <div class="control">
          <label for="thickness">Thickness</label>
          <input
            type="range"
            min="1"
            max="10"
            v-model="thickness"
            @input="updateThickness"
            title="Thickness"
          />
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        distance: 46,
        thickness: 3,
      };
    },
    methods: {
      updateDistance() {
        this.$refs.wrap.style.setProperty(
          '--distance',
          `${this.distance}%`
        );
      },
      updateThickness() {
        this.$refs.wrap.style.setProperty(
          '--border',
          `${this.thickness}px`
        );
      },
    },
  };
  </script>
  
  <style scoped>
  :root {
    --border: 3px;
    --color1: #6be89b;
    --color2: #0076a5;
    --from: 30deg;
    --distance: 46%;
  }
  
  body {
    background: #33353d;
    display: grid;
    place-items: center;
    height: 100vh;
    margin: 0;
  }
  
  .img-wrap {
    position: relative;
    padding: 30px;
  }
  
  .img-wrap::after {
    content: '';
    border-radius: 999px;
    display: block;
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    background: conic-gradient(
      from var(--from),
      var(--color1),
      var(--color2) var(--distance),
      transparent var(--distance)
    );
    -webkit-mask: radial-gradient(
      farthest-side,
      transparent calc(100% - var(--border)),
      #fff calc(100% - var(--border) + 1px)
    );
    mask: radial-gradient(
      farthest-side,
      transparent calc(100% - var(--border)),
      #fff calc(100% - var(--border) + 1px)
    );
  }
  
  img {
    border-radius: 999px;
    display: block;
    width: calc(100vw - 80px);
    max-width: 360px;
  }
  
  /* CONTROLS */
  .controls {
    position: absolute;
    top: 0.5em;
    right: 0.5em;
    background: #000a;
    padding: 0.5em;
    display: grid;
    gap: 0.25em;
    color: #eee;
    font-family: system-ui, sans-serif;
    font-size: 0.875rem;
    text-transform: uppercase;
  }
  
  .control {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 1em;
  }
  
  input {
    width: 200px;
  }
  </style>
  