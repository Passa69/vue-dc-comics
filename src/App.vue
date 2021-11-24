<template>
  <div id="app">
    <!-- componente header -->
    <Header/>

    <!-- main -->
    <main>
      <!-- componenti main -->
      <Content/>
      <Elements/>
    </main>

    <!-- footer -->
    <footer>
      <!-- componenti footer -->
      <FooterUp/>
      <FooterDown/>
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Content from './components/Content.vue';
import Elements from './components/Elements.vue';
import FooterUp from './components/FooterUp.vue';
import FooterDown from './components/FooterDown.vue';

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Elements,
    FooterUp,
    FooterDown
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
}
</style>
