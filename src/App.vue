<template>
  <v-app>
    <div class="wrapper">
      <NavBarMobile></NavBarMobile>
      <Navbar></Navbar>
      <Header></Header>
      <v-content>
        <router-view></router-view>
      </v-content>
    </div>
  </v-app>
</template>

<script>
import NavBarMobile from "./components/NavBarMobile.vue";
import Navbar from "./components/Navbar.vue";
import Header from "./components/Header.vue";
export default {
  name: "App",
  components: { NavBarMobile, Navbar, Header },
  data() {
    return {
      //
    };
  }
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=PT+Sans');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'PT Sans', sans-serif;

}

.application--wrap{
  background-color:#262626;
}
</style>

