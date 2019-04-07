<template>
  <div class="app-footer">
    <address>
      <p>ul. Jakas tam</p>
      <p>00-000 Warszawa</p>
      <p class="mobile-contact">
        <v-icon>smartphone</v-icon>601-601-601
      </p>
    </address>

    <a href="https://www.instagram.com/nails_by_dzoana_/?hl=pl">
      <img src="../assets/instagram.png">
    </a>

    <p>design by lbogacz</p>
    <p>&copy; 2019</p>

    <div class="app-footer-map">
      <iframe
        class="hidden-sm-and-down"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d156388.35438504175!2d20.921112620236695!3d52.233065320878424!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x471ecc669a869f01%3A0x72f0be2a88ead3fc!2sWarsaw%2C+Poland!5e0!3m2!1sen!2suk!4v1554327787675!5m2!1sen!2suk"
        frameborder="0"
        allowfullscreen
      ></iframe>
    </div>
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
  font-size: 15px;
  address {
    text-align: right;
    padding: 5px;
  }
  img {
    height: 50px;
    width: 50px;
    position: relative;
    top: -80px;
    left: 15px;
  }
  p {
    margin: 0 0 5px 3px;
  }
  a {
    cursor: pointer;
  }
  iframe {
    width: 100%;
    height: 150px;
    border: 0;
    margin-top: 20px;
  }
}

@media (min-width: 400px) {
  .app-footer {
    height: 250px;
  }
}

@media (min-width: 450px) {
  .app-footer {
    height: 350px;
    margin-bottom: 5px;
    address {
      position: relative;
      top: -50px;
      right: 15px;
    }
    img {
      top: -50px;
    }
    p {
      position: relative;
      top: 150px;
    }
  }
}

@media (min-width: 650px) {
  .app-footer {
    height: 400px;
    img {
      height: 60px;
      width: 60px;
    }
    address,
    p {
      font-size: 20px;
    }
  }
}

@media (min-width: 850px) {
  .app-footer {
    height: 450px;
    img {
      height: 70px;
      width: 70px;
      left:50px;
    }
    address{
      right:60px;
    }
    p {
      top:180px;
    }
  }
}

@media (min-width: 650px) {
.app-footer{
  iframe{
    margin-top: 190px;
    height: 350px;

  }
}
}
</style>
