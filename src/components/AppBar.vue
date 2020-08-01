<template>
  <v-app-bar
    color="orange darken-3"
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
    <div v-for="item in navbar_items" :key="item">
      <v-btn
      text
      class="subheading mr-4 hidden-xs-only"
      color="white"
    >
      {{ item }}
    </v-btn>
    </div>
  </v-app-bar>
</template>

<script>
  // // Utilities
  // import {
  //   mapMutations,
  //   mapState,
  // } from 'vuex'

  export default {
    name: 'CoreAppBar',

    data: () => ({
      hasColor: false,
      navbar_items: [
          'Home',
          'Login',
          'Register',
          'About',
          'Student',
      ]
    }),

    computed: {
      // ...mapState('app', ['links']),
      // color () {
      //   return this.hasColor ? 'orange darken-3' : 'orange darken-3'
      // },
    },
    methods: {
      // ...mapMutations('app', ['toggleDrawer']),
      // onScroll () {
      //   this.hasColor = window.scrollY > 30
      // },
    },
  }
</script>
