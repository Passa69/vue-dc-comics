<template>
  <section>
      <div>
        <ul class="items">
          <li v-for="(item, i) in mainItems" :key="i">
            <img :src="require(`../assets/img/${item.img}`)" alt="">

            <span>{{ item.title }}</span>
          </li>
        </ul>
        
      </div>
  </section>
</template>

<script>
export default {
  name: 'Elements',
  data() {
    return {
      mainItems: [
        {
          img: "buy-comics-digital-comics.png",
          title: "DIGITAL COMICS",
        },
        {
          img: "buy-comics-merchandise.png",
          title: "DC MERCHANDISE",
        },
        {
          img: "buy-comics-shop-locator.png",
          title: "SUBSCRIPTION",
        },
        {
          img: "buy-comics-subscriptions.png",
          title: "COMIC SHOP LOCATOR",
        },
        {
          img: "buy-dc-power-visa.svg",
          title: "DC POWER VISA",
        }
      ]
    }
  }
 }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
  background-color: #0282f9;
  height: 150px;
}

.items {
  margin: 0 auto;
  list-style-type: none;
  display: flex;
  align-items: center;
}

img {
  width: 50px;
  vertical-align: center;
}

ul {
  padding-top: 30px;
}

li {
  margin: 0 50px;
}

span {
  color: white;
}
</style>