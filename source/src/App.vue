<template>
  <Navbar :logo="logo_src" :alt="alt_name_src" />
  <router-view />
  <Footer />
</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    Navbar,
    Footer
  },

  data() {
    return {
      logo_src: "/img/logo.png",
      alt_name_src: "Logo da Página"
    }
  }
}

</script>

<style>
* {
  font-family: Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  /**Não passar da largura máxima da div pai*/
}

.main-container {
  margin: 50px;
  min-height: 250px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>