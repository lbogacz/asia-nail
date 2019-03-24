<template>
  <div class="app-home">

    <div class="app-home-header">
      <h2>Welcome message</h2>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quidem, tempora recusandae reiciendis sequi enim nihil sapiente quasi laboriosam nam doloremque consequuntur, dolorem sit fugiat voluptatibus ut eaque, impedit sed vero.</p>
      <router-link :to='{name:"service"}'>
        <v-btn>Wiecej...</v-btn>
      </router-link>
    </div>

    <div class="app-home-content">
    <h2>Manicure</h2>
    <img src="../assets/pexels-photo-361754.jpeg" alt="manicure">
    <router-link :to='{name:"service"}'>
        <v-btn>Wiecej...</v-btn>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",

  data() {
    return {};
  }
};
</script>
 <style lang="scss" scoped>
.app-home {
  text-align: center;
}

.app-home-header {
padding:30px;
  h2 {
    color: #fff;
    font-size: 24px;
    padding: 10px 2px;
  }
  p {
    color: #959595;
    font-size: 14px;
  }
}

 a {
    text-decoration: none;
  }

  .app-home-content{
    padding:30px;

    color: #fff;
    h2{
    padding: 10px 2px;
    }
    img{
    height:200px;
    width:100%;
    object-fit: cover;
    }
    button{
      margin-top:15px;
    }
  }
</style>
