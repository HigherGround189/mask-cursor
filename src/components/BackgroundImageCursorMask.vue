<template>
  <div @mousemove="updateCursorPosition">
    <CursorMask
      :mouseX="mouseX"
      :mouseY="mouseY"
      :imageSrc="imageSrc"
      />
    <BackgroundImage :imageSrc="imageSrc"/>
  </div>
</template>

<script>
import BackgroundImage from './BackgroundImage.vue';
import CursorMask from './CursorMask.vue';

  export default {
    components: { BackgroundImage, CursorMask },
    props: ["imageSrc"],
    data() {
      return {
        mouseX: 0,
        mouseY: 0
      }
    },
    methods: {
      updateCursorPosition(event) {
        this.mouseX = event.clientX
        this.mouseY = event.clientY
      }
    }
  }
</script>

<style scoped>
  div {
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;

  }

  div > * {
    grid-row: 1 / 2;
    grid-column: 1 / 2;
  }
</style>
