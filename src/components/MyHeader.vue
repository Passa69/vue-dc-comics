<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="">

    <nav>
      <ul>
        <li v-for="(links, i) in navHeader" :key="i">
          <a href="links.link" :class="links.here? 'selected' : ''">{{ links.name }}</a>
        </li>
      </ul>
    </nav>
    
  </header>
</template>

<script>
export default {
  name: 'MyHeader',
  data() {
    return {
        navHeader: [
        {
          name: "Characters",
          link: "#",
          here: false
        },
        {
          name: "Comics",
          link: "#",
          here: true
        },
        {
          name: "Movies",
          link: "#",
          here: false
        },
        {
          name: "TV",
          link: "#",
          here: false
        },
        {
          name: "Games",
          link: "#",
          here: false
        },
        {
          name: "Collectibles",
          link: "#",
          here: false
        },
        {
          name: "Videos",
          link: "#",
          here: false
        },
        {
          name: "Fans",
          link: "#",
          here: false
        },
        {
          name: "News",
          link: "#",
          here: false
        },
        {
          name: "Shop",
          link: "#",
          here: false
        }
      ]
    }
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  margin: 0 auto;
  width: 80%;
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  li {
    display: inline-block;
    margin: 0 10px;

    a {
      color: black;
      text-decoration: none;
      padding: 0 5px 20px 5px;

      &.selected {
        color: #3190f9;
        border-bottom: 4px solid #3190f9;
      }
    }
  }
}
</style>
