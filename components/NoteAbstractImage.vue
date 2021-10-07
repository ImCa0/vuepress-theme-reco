<template>
  <div v-if="item.frontmatter.abs_img">
    <img :src="item.frontmatter.abs_img" alt="abc">
  </div>
</template>

<script>
export default {
  name: 'NotePic',
  props: ['item']
}
</script>

<style lang="stylus" scoped>
img
  width: 100%;
  background-size: contain;
  background-repeat: no-repeat;
  border-radius: $borderRadius;
  box-shadow: var(--box-shadow);
</style>