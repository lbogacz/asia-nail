<template>
  <nav>
    <v-toolbar dark>
      <v-toolbar-side-icon @click="drawer=!drawer"></v-toolbar-side-icon>
    </v-toolbar>

    <v-navigation-drawer dark v-model="drawer" app>
      <v-list>
        <v-list-tile v-for="link in links" :key="link.text" router :to="link.route">
          <v-list-tile-action>
            <v-icon>{{links.icon}}</v-icon>
          </v-list-tile-action>

          <v-list-tile-content>
            <v-list-tile-title>{{link.text}}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      drawer: false,
      links: [
        { icon: "", text: "Strona Domowa", route: "/" },
        { icon: "", text: "Galeria", route: "/gallery" },
        { icon: "", text: "Usługi", route: "/service" },
        { icon: "", text: "O mnie", route: "/about" }
      ]
    };
  }
};
</script>