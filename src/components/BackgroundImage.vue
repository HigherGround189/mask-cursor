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
  }

  img {
    width: inherit;
    height: inherit;
  }
</style>
