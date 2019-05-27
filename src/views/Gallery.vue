<template>
  <div class="gallery">
    <gallery-item v-for="i in 10" :key="i"></gallery-item>
  </div>
</template>

<script>
import GalleryItem from '@/components/GalleryItem.vue';

export default {
  components: { GalleryItem },
};
</script>

<style lang="sass" scoped>
  .gallery
    display: flex
    width: auto
    height: 100vh
    padding: 56px
    column-width: 50px
    column-gap: 12px
    column-fill: balance
</style>
