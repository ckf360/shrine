<template>
  <div id="app" class="background--primary">
    <navbar></navbar>
    <div class="view">
      <router-view class="view__page"/>
    </div>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue';

export default {
  name: 'App',
  components: {
    Navbar,
  },
};
</script>

<style lang="sass" scoped>
  @import ./assets/sass/colors

  .view
    filter: drop-shadow(-1px -1px 3px darken($primary, 7%));
    .view__page
      background-color: white
      clip-path: polygon(50px 0, 100% 0, 100% 100%, 0 100%, 0 50px)
      width: 2000px
</style>
