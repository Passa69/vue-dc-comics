<template>
  <div id="app">
    <!-- componente header -->
    <Header/>

    <!-- main -->
    <main>
      <!-- componenti main -->
    </main>

    <!-- footer -->
    <footer>
      <!-- componenti footer -->
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
