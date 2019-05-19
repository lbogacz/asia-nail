<template>
  <div class="app-header">
    <div class="app-header-mobile">
      <img src="../assets/pexels-photo-1889347.jpeg" alt="black women">
    </div>

    <div class="app-header-desktop">
      <v-parallax :src="require('@/assets/pexels-photo-1889347.jpeg')" height="800"></v-parallax>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style lang="scss" scoped>
.app-header-mobile {
  img {
    margin-top: 50px;
    height: 450px;
    width: 100%;
    object-fit: cover;
    @media (min-width: 425px) {
      height: 550px;
    }
    @media (min-width: 520px) {
      height: 650px;
    }
    @media (min-width: 620px) {
      height: 750px;
    }
    @media (min-width: 720px) {
      height: 850px;
    }
    @media (min-width: 820px) {
      height: 990px;
    }
    @media (min-width: 960px) {
      display: none;
    }
  }
}

.app-header-desktop {
  @media (max-width: 959px) {
    display: none;
  }
  @media (min-width: 960px) {
    object-fit: contain;
  }
}
</style>
