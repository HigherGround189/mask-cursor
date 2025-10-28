<template>
  <div :style="{
    backgroundImage: `url(${imageSrc})`,
    top: `${mouseY}px`,
    left: `${mouseX}px`,
    backgroundPosition: `-${mouseX}px -${mouseY}px`
  }">
  </div>
</template>

<script>
  export default {
    props: ["mouseX", "mouseY", "imageSrc"]
  }
</script>

<style scoped>
  div {
    width: 10vw;
    aspect-ratio: 1 / 1;
    overflow: hidden;
    position: absolute;
    transform: translate(-50%, -50%);
    z-index: 1;
    border-radius: 50%;
    background-size: cover;
    filter: invert(1);
    transition: 0.1s;
    background-repeat: no-repeat;
    background-size: 100vw 100vh;
    background-color: red;
  }
</style>
