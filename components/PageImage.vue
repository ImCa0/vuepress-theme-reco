<template>
  <div class="page-image" v-if="$page.frontmatter.head_img">
    <img :src="$page.frontmatter.head_img" alt="">
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.page-image {
  overflow: hidden;
}
img {
  width: 100vw;
}
@media (min-width: 1024px) {
  .page-image {
    height: calc(100vh - 3.6rem);
    position: relative;
  }
  img {
    position: absolute;  
    top: 0;  
    bottom: 0;  
    left: 0;  
    right: 0;  
    margin: auto;
  }
}
</style>