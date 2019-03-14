<template>
  <div class="header">
    <div class="header-mobile">
      <img src="../assets/pexels-photo-1889347.jpeg" alt="black women">
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style lang="scss" scoped>
.header-mobile {
  img {
      margin-top:50px;
    height: 450px;
    width: 100%;
    object-fit: cover;
  }
}
</style>
