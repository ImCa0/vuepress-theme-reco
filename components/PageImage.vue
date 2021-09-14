<template>
  <div class="page-image" v-if="$page.frontmatter.pic">
    <img :src="$page.frontmatter.pic" alt="">
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
  }
}
</style>