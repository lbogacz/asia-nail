<template>
  <v-toolbar class="hidden-sm-and-down" dark fixed scroll-off-screen scroll-threshold="1">
    <v-spacer></v-spacer>
    <v-toolbar-items>
      <v-btn flat v-for="link in links" :key="link.text" route :to="link.route">{{link.text}}</v-btn>
    </v-toolbar-items>
  </v-toolbar>

</template>

<script>
export default {
    name:"Navbar",
    data(){
        return{
            links:[
                { text: "Strona Domowa", route: "/" },
                { text: "Galeria", route: "/gallery" },
                { text: "Usługi", route: "/service" },
                { text: "O mnie", route: "/about" }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
// .v-toolbar{
//   top:850px;
// }
</style>
