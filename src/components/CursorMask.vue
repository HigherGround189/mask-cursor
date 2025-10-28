<template>
  <div>
    <img :src="this.$props.imageSrc" alt=""/>
  </div>
</template>

<script>
  export default {
    props: ["imageSrc"]
  }
</script>

<style scoped>
  div {
    width: 100vw;
    height: 100vh;
    overflow: hidden;
    z-index: 1;
  }

  img {
    width: inherit;
    height: inherit;
    filter: invert(1);
  }
</style>
