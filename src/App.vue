<template>
  <v-app>
    <NavBar></NavBar>
    <Header></Header>
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Header from "./components/Header.vue";
export default {
  name: "App",
  components: { NavBar, Header },
  data() {
    return {
      //
    };
  }
};
</script>

<style lang="scss">
*{
  margin:0;
  padding:0;
  box-sizing: border-box;
}
</style>

