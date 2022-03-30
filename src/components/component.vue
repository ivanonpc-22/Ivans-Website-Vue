<template>
  <div class="component-container">
    <img :alt="image_alt" :src="image_src" class="component-image" />
  </div>
</template>

<script>
export default {
  name: 'AppComponent',
  props: {
    image_src: {
      type: String,
      default: '/playground_assets/download-200h.png',
    },
    image_alt: {
      type: String,
      default: 'image',
    },
  },
}
</script>

<style scoped>
.component-container {
  display: flex;
  position: relative;
}
.component-image {
  width: 40px;
  height: 40px;
  object-fit: cover;
}
</style>
