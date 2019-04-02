<template>
  <div class="app-footer">

    <address>
      <p>ul. Jakas tam</p>
      <p>00-000 Warszawa</p>
      <p class="mobile-contact">
        <v-icon>smartphone</v-icon>601-601-601
      </p>
    </address>

    <a href="https://www.instagram.com/nails_by_dzoana_/?hl=pl"> <img src="../assets/instagram.png"></a>

    <p>design by lbogacz</p>
    <p>&copy; 2019</p>
  </div>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style lang="scss" scoped>
.app-footer {
  height: 220px;
  width: 100%;
  background: url("../assets/nail-varnish-3928384_1920.jpg") no-repeat;
  background-size: cover;
  background-position: center;
  opacity: 0.5;
  font-size:15px;
  address {
    text-align: right;
    padding: 5px;
  }
  img{
    height:50px;
    width: 50px;
    position:relative;
    top:-80px;
    left:15px;
  }
  p{
    margin-bottom:5px;
  }
  a{
    cursor: pointer;
  }
}
</style>
