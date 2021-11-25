<template>
  <footer>
    <button>SIGN-UP NOW!</button>

    <div class="social">
        <h4>FOLLOW US</h4>
        <img src="../assets/img/footer-facebook.png" alt="">
        <img src="../assets/img/footer-periscope.png" alt="">
        <img src="../assets/img/footer-pinterest.png" alt="">
        <img src="../assets/img/footer-twitter.png" alt="">
        <img src="../assets/img/footer-youtube.png" alt="">
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterDown',
 }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
footer {
    background-color: #303030;
    height: 100px;
    padding: 0 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

button {
    margin-left: 20px;
    background-color: #303030;
    color: white;
    border: 1px solid #145fa5;
    padding: 20px 10px;
}

.social {
    display: flex;
    margin-right: 20px;
}

.social img{
    height: 30px;
    width: 30px;
    margin: 15px 10px;
}

h4 {
    margin: 20px;
    color: #0a78f3;
}
</style>