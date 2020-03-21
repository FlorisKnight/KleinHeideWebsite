<template>
 <div class="PictureDivider" :style="backgroundStyle"></div>
</template>

<script>
export default {
  name: 'PictureDivider',
  props: {
    url: String,
  },
  computed: {
    backgroundStyle() {
      return {
        'background-image': `linear-gradient(120deg,
        rgba(212, 252, 121, 0.5) 0%,
        rgba(150, 230, 161, 0.5) 100%) , url(${this.url})`,
      };
    },
  },
};
</script>

<style scoped>
.PictureDivider {
  background: #464646 no-repeat center center;
  background-size: cover;
  height: 60vh;
}
</style>
