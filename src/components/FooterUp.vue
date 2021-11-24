<template>
  <footer>
    <div class="elem">
        <div>
            <ul>
                <h4>DC Comics</h4>
                <li v-for="(option, i) in Comics" :key="i">
                    <a href="#">{{ option }}</a>
                </li>
            </ul>
            <ul>
                <h4>Shop</h4>
                <li v-for="(option, i) in Shop" :key="i">
                    <a href="#">{{ option }}</a>
                </li>
            </ul>
        </div>

        <ul>
            <h4>DC</h4>
            <li v-for="(option, i) in DC" :key="i">
                <a href="#">{{ option }}</a>
            </li>
        </ul>
        <ul>
            <h4>Sites</h4>
            <li v-for="(option, i) in Sites" :key="i">
                <a href="#">{{ option }}</a>
            </li>
        </ul>
    </div>

    <img src="../assets/img/dc-logo-bg.png" alt="">
    
  </footer>
</template>

<script>
export default {
  name: 'FooterUp',
  data() {
      return {
        Comics: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Videos",
            "News"
        ],
        Shop: [
            "Shop DC",
            "Shop DC Collectibles"
        ],
        DC: [
            "Terms Of Use",
            "Privacy policy (New)",
            "Ad Choices",
            "Advertising",
            "Jobs",
            "Subscriptions",
            "Talent Workshops",
            "CPSC Certificates",
            "Ratings",
            "Shop Help",
            "Contact Us"
        ],
        Sites: [
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC Universe",
            "DC Power Visa"
        ]
      }
  }
 }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
footer {
    background-image: url('../assets/img/footer-bg.jpg');
    margin-top: 50px;
    display: flex;
    justify-content: space-between;

    h4 {
       text-align: left;
       color: white; 
    }

    ul {
        list-style-type: none;
    }

    li {
        margin: 10px;
        text-align: left;
        font-size: 10px;

        a {
            color: #555350;
            text-decoration: none;
        }
    }
}

.elem {
        display: flex;
}

img {
    margin-right: 400px;
    padding: 20px;
    height: 300px;
}
</style>