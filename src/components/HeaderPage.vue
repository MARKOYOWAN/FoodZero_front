<template>
  <div class="background">
    <div class="header">
      <b-dropdown
        id="dropdown-1"
        variant="outline-light"
        text="FoodZero"
        no-caret
        class="logo"
      >
        <b-dropdown-item>First Action</b-dropdown-item>
        <b-dropdown-item>Second Action</b-dropdown-item>
        <b-dropdown-item>Third Action</b-dropdown-item>
      </b-dropdown>
      <div class="header-right">
        <a href="#contact">+86 852 346 000</a>
        <b-button variant="outline-light">Button</b-button>
      </div>
    </div>

    <div class="title">
      <p>Deep Sea Snow white</p>
      <p>Cod Fillet</p>
    </div>
      <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "HeaderPage",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
* {
  box-sizing: border-box;
}

.title {
  font-size: 45px;
  text-align: center;
  color: white;
  line-height: 34px;
  margin-top: 90px;
}

.background {
  background: transparent url(../assets/images/fruit.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 40vh;
}
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}

.header {
  padding: 20px 50px;
}

.header a {
  float: left;
  color: white;
  text-align: center;
  padding: 7px;
  text-decoration: none;
  font-size: 18px;
  line-height: 25px;
  border-radius: 4px;
  font-weight: bolder;
}

.header a.logo {
  font-size: 25px;
  font-weight: bold;
}

.header a:hover {
  background-color: #ddd;
  color: black;
}

.header a.active {
  background-color: dodgerblue;
  color: white;
}

.header-right {
  float: right;
}

@media screen and (max-width: 500px) {
  .header a {
    float: none;
    display: block;
    text-align: left;
  }

  .header-right {
    float: none;
  }
}
</style>
