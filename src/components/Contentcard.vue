<template>
  <section>
      <div>
          <img :src="details.thumb" alt="">
          <p>{{ details.series }}</p>
      </div>
  </section>
</template>

<script>
export default {
  name: 'Contentcard',
  props: {
      details: Object
  }
 }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {

    div {
        margin: 25px 20px;
        height: 150px;
        width: 150px;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }

        p {
            font-size: 15px;
            color: white;
        }
    }
}


</style>