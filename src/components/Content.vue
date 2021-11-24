<template>
  <section>
      <h1>--> Content goes here</h1>
  </section>
</template>

<script>
export default {
  name: 'Content',
 }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
  margin-top: 10px;
  background-color: #1c1c1c;
  height: 100px;
  display: flex;
  align-items: center;

  h1 {
    color: white;
    margin-left: 100px;
  }
}
</style>