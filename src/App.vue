<template>
  <div id="app">
    <!-- componente header -->
    <MyHeader/>

    <!-- main -->
    <main>
      <!-- componenti main -->
      <Content/>
      <Elements/>
    </main>

    <!-- footer -->
    <footer>
      <!-- componenti footer -->
      <MyFooterUp/>
      <MyFooterDown/>
    </footer>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import Content from './components/Content.vue';
import Elements from './components/Elements.vue';
import MyFooterUp from './components/MyFooterUp.vue';
import MyFooterDown from './components/MyFooterDown.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    Content,
    Elements,
    MyFooterUp,
    MyFooterDown
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

main {
  margin-top: 20px;
  background-color: #1c1c1c;
}
</style>
