<template>
  <footer>
    <p>&copy; 2024 FizjoStacja. Wszelkie prawa zastrzeżone.</p>
  </footer>
</template>
  
<script>

export default {
  components: {},
  methods: {
    goTop() {
      section.scrollIntoView({ behavior: 'smooth' });
    },

  }
};
</script>
  
<style lang="scss" scoped>


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

}
</style>
  