<template>
  <div id="app">

    <!-- HEADER -->
    <Header/>

    <!-- MAIN -->
    <Main/>

    <!-- FOOTER -->
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/Header.vue"
import Main from "@/components/Main.vue"
import Footer from "@/components/Footer.vue"
export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
  /* UTILITIES GENERAL */
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  #app{
    max-width: 100%;
  }

  header,
  main,
  footer{
    max-width: 100%;
  }

  li{
    list-style: none;
  }

  a{
    text-decoration: none;
  }
</style>
