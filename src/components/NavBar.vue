<template>
  <nav>
    <v-menu offset-y dark >
      <template v-slot:activator="{ on }">
        <v-toolbar dark flat>
          <v-toolbar-side-icon v-on="on"></v-toolbar-side-icon>
        </v-toolbar>
      </template>

      <v-list>
        <v-list-tile v-for="link in links" :key="link.text" @click="menu = !menu" route :to="link.route">
          <v-list-tile-title>{{ link.text }}</v-list-tile-title>
        </v-list-tile>
      </v-list>
    </v-menu>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      menu: false,
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