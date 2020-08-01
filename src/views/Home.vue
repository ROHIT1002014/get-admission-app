<template>
  <div class="home">
      <banner />
      <Colleges />
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from '@/components/Banner.vue';
import Colleges from '@/components/Colleges.vue';

export default {
  name: 'Home',
  components: {
    Banner,
    Colleges,
  }
}
</script>
