<template>
  <div id="app">
    <!-- componente header -->
    <MyHeader/>

    <!-- main -->
    <main>
      <!-- componenti main -->
      <Jumbotron/>
      <h2>CURRENT SERIES</h2>
      <Content/>
      <button>LOAD MORE</button>
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
import Jumbotron from './components/Jumbotron.vue';
import Content from './components/Content.vue';
import Elements from './components/Elements.vue';
import MyFooterUp from './components/MyFooterUp.vue';
import MyFooterDown from './components/MyFooterDown.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    Jumbotron,
    Content,
    Elements,
    MyFooterUp,
    MyFooterDown
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

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

  h2 {
    color: white;
    background-color: #0282f9;
    padding: 10px;
    margin-left: 150px;
    width: 250px;
  }

  button {
    color: white;
    background-color: #0282f9;
    border: inherit;
    padding: 10px;
    margin-bottom: 25px;
  }
}
</style>
