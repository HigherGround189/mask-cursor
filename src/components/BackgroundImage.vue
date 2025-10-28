<template>
  <div :style="{ backgroundImage: `url(${imageSrc})` }">
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
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
  }
</style>
