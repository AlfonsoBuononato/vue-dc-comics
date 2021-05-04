<template>
  <div id="app">

    <!-- HEADER -->
    <Header/>

    <!-- MAIN -->
    <Main/>

    <!-- FOOTER -->
    <footer>qui footer</footer>
  </div>
</template>

<script>
import Header from "@/components/Header.vue"
import Main from "@/components/Main.vue"
export default {
  name: 'App',
  components: {
    Header,
    Main,
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
    max-width: 1200px;
    margin: auto;
  }
</style>
