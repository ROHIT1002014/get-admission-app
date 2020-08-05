<template>
  <v-app-bar
    style="background-color:red;"
    app
    elevate-on-scroll
  >
    <h4 class="font-weight-bold white--text">
      VUETIFY
    </h4>
    <h4 class="font-weight-light white--text">
      MATERIALKIT
    </h4>
    <v-spacer class="hidden-xs-only" />
      <nav role="navigation">
        <ul>
          <li><a href="#"><v-icon class="mr-1">mdi-home</v-icon>home</a></li>
          <li><a href="#">colleges<v-icon color="white" style="font-size:30px">mdi-chevron-down</v-icon> </a>
            <ul class="dropdown">
              <li><a href="#">One  jhbj kj b kb Sub-1</a></li>
              <li><a href="#">Sub-2 One  jhbj kj b kb </a></li>
              <li><a href="#">Sub-3 One  jhbj kj b kb </a></li>
            </ul>
          </li>
          <li><a href="#">Admission<v-icon color="white" style="font-size:30px">mdi-chevron-down</v-icon></a>
          <ul class="dropdown">
              <li><a href="#">One  jhbj kj b kb Sub-1</a></li>
              <li><a href="#">Sub-2 One  jhbj kj b kb </a></li>
              <li><a href="#">Sub-3 One  jhbj kj b kb </a></li>
            </ul>
          </li>
          <li><a href="#">school</a></li>
          <li><a href="#"><v-icon class="mr-1">mdi-login</v-icon>login</a></li>
          <li><a href="#"><v-icon class="mr-1">mdi-file-document</v-icon>Register</a></li>
          <li><a href="#"><v-icon class="mr-1">mdi-human-greeting</v-icon>about</a></li>
        </ul>
    </nav>
    <!-- <div v-for="item in navbar_items" :key="item">
      <v-btn
      text
      class="subheading mr-4 hidden-xs-only"
      color="white"
    >
      {{ item }}
    </v-btn>
    </div> -->
  </v-app-bar>
</template>
<script>
  export default {
    data: () => ({
      navbar_items: [
          'Home',
          'Login',
          'Register',
          'About',
          'Student',
      ],
      admins: [
        ['Management'],
        ['Settings'],
      ],
      cruds: [
        ['Create'],
        ['Read'],
        ['Update'],
        ['Delete'],
      ],
    }),
  }
</script>
<style scoped>
a {
  text-decoration: none;
}

nav {
    text-transform: uppercase;
    font-weight: bold;
}

ul {
  background: rgb(190, 165, 22);
  list-style: none;
  margin: 0;
  padding-left: 0;
}

li {
  color: #fff;
  background: red;
  display: block;
  float: left;
  padding: 1rem;
  position: relative;
  text-decoration: none;
  transition-duration: 0.5s;
}

li a {
  color: #fff;
}

li:hover {
    background: rgb(255, 115, 0);
    cursor: pointer;
}

ul li ul {
  background: orange;
  visibility: hidden;
  opacity: 0;
  min-width: 5rem;
  position: absolute;
  transition: all 0.5s ease;
  margin-top: 1rem;
  left: 0;
  display: none;
}

ul li:hover > ul,
ul li ul:hover {
  visibility: visible;
  opacity: 1;
  display: block;
}

ul li ul li {
  clear: both;
  width: 100%;
  height: auto;
}
</style>