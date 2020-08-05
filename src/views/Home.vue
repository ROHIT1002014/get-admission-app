<template>
  <div class="home">
      <banner />
      <v-parallax
        height="auto"
        src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
      >
        <h1>Universities:</h1>
        <Universities />
        <h1>Colleges:</h1>
        <Colleges />
        <h1>Schools:</h1>
        <Schools />
        <h1>Professional Courses:</h1>
        <Courses />
      </v-parallax>
      <Review />
      <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from '@/components/Banner.vue';
import Colleges from '@/components/Colleges.vue';
import Schools from '@/components/School.vue';
import Universities from '@/components/Universities.vue';
import Courses from '@/components/Courses.vue';
import Review from '@/components/Review.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'Home',
  components: {
    Banner,
    Colleges,
    Schools,
    Universities,
    Courses,
    Review,
    Footer,
  }
}
</script>
