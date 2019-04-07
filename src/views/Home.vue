<template>
  <div class="app-home">
    <Header></Header>
    <div class="app-home-header">
      <h2>Welcome message</h2>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quidem, tempora recusandae reiciendis sequi enim nihil sapiente quasi laboriosam nam doloremque consequuntur, dolorem sit fugiat voluptatibus ut eaque, impedit sed vero.</p>
      <router-link :to='{name:"service"}'>
        <v-btn>Wiecej...</v-btn>
      </router-link>
    </div>

    <div class="app-home-content">
      <div class="app-home-content-manicure">
        <h2>Manicure</h2>
        <img src="../assets/pexels-photo-361754.jpeg" alt="manicure">
        <router-link :to='{name:"service"}'>
          <v-btn color="purple darken-1">Wiecej...</v-btn>
        </router-link>
      </div>

      <div class="app-home-content-manicureArt">
        <h2>Manicure Art</h2>
        <img src="../assets/beauty-fingernails-hearts-37553.jpg" alt="manicure art">
        <router-link :to='{name:"service"}'>
          <v-btn color="pink accent-1">Wiecej...</v-btn>
        </router-link>
      </div>

      <div class="app-home-content-repair">
        <h2>Naprawa</h2>
        <img src="../assets/pexels-photo-887352.jpeg" alt="repair nail">
        <router-link :to='{name:"service"}'>
          <v-btn color="#B6254A">Wiecej...</v-btn>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
export default {
  name: "Home",
  components: { Header },
  data() {
    return {};
  }
};
</script>
 <style lang="scss" scoped>
.app-home {
  text-align: center;
  color: #fff;
}

.app-home-content-manicure,
.app-home-content-manicureArt,
.app-home-content-repair {
  margin-bottom: 30px;
}
.app-home-header,
.app-home-content-manicure,
.app-home-content-manicureArt,
.app-home-content-repair {
  padding: 30px;
}

h2 {
  padding: 10px 2px;
}

.app-home-header {
  margin-bottom: 30px;
  h2 {
    font-size: 24px;
  }
  p {
    color: #959595;
    font-size: 14px;
  }
}

a {
  text-decoration: none;
}

.app-home-content {
  img {
    height: 200px;
    width: 100%;
    object-fit: cover;
  }
  button {
    margin-top: 15px;
  }
}

.app-home-content-manicure {
  h2 {
    color: #8e24aa;
  }
}

.app-home-content-manicureArt {
  h2 {
    color: #ff80ab;
  }
}
.app-home-content-repair {
  h2 {
    color: #b6254a;
  }
}

@media (min-width: 500px) {
  .app-home-content {
    img {
      height: 250px;
    }
  }
}

@media (min-width: 600px) {
  .app-home-content {
    img {
      height: 300px;
    }
  }
}

@media (min-width: 700px) {
  .app-home-content {
    img {
      height: 350px;
    }
  }
}

@media (min-width: 800px) {
  .app-home-content {
    img {
      height: 400px;
    }
  }
}
</style>
