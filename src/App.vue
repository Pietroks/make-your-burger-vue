<template>
    <div>
      <NavBar :logo="logo_scr" :alt="app_name"/>
      <RouterView/>
      <Footer/>
    </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import { RouterView } from 'vue-router';
import Footer from './components/Footer.vue';


export default {
  components: {
    RouterView,
    NavBar,
    Footer
  },
  data() {
    return {
      logo_scr: '/img/logo.png',
      app_name: 'Make Your Burguer'
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
