<template>
  <Header/>
  <Main/>
  <Footer/>
</template>
<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style>
body{
  width:100vw;
  height:100vh;
  margin:0;
}

#app{
  width:100%;
  height:100%;
  margin:0;
}

</style>
