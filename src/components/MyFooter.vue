<template>
  <footer>
    <p>&copy; 2024 FizjoStacja. Wszelkie prawa zastrzeżone.</p>

    

    <!-- <div class="pote">
      <button @click="openModal">
        <h1>
          potrzebujesz strony?
        </h1>
      </button>
      <div id="modal">
        <Modal ref="modalRef" />
      </div>
    </div> -->
  </footer>
</template>
  
<script>

import Modal from "./PoteModal.vue";

export default {
  components: {
    Modal
  },
  methods: {
    openModal() {
      this.$refs.modalRef.openModal();

      setTimeout(() => {
        this.goTop();
      }, 50);

    },
    goTop() {
      const section = document.getElementById('modal');
      section.scrollIntoView({ behavior: 'smooth' });
    },

  }
};
</script>
  
<style lang="scss" scoped>
@keyframes color {
  0% {
    border-color: #33CCCC;
  }

  20% {
    border-color: #33CC36;
  }

  40% {
    border-color: #B8CC33;
  }

  60% {
    border-color: #FCCA00;
  }

  80% {
    border-color: #33CC36;
  }

  100% {
    border-color: #33CCCC;
  }
}

footer {
  background-color: #333;
  background-image: linear-gradient(80deg, #52e3593f 10%, #38456757 100%);
  color: #fff;
  padding: 20px 0;
  margin-top: 30px;
  bottom: 0;
  width: 100%;
  text-align: center;

  p {
    font-size: small;
  }

  .pote {

    display: flex;
    flex-direction: column;
    align-items: center;

    button {
      background: none;
      border-radius: 15px;
      border-color: greenyellow;
      padding: 0 12px 0 12px;

      animation: color 5s infinite linear;

    }


    button:hover {
      cursor: pointer;
    }
  }
}
</style>
  