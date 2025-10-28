<template>
  <div>
    <CursorMask :imageSrc="this.$props.imageSrc"/>
    <BackgroundImage :imageSrc="this.$props.imageSrc"/>
  </div>
</template>

<script>
import BackgroundImage from './BackgroundImage.vue';
import CursorMask from './CursorMask.vue';

  export default {
    components: { BackgroundImage, CursorMask },
    props: ["imageSrc"]
  }
</script>

<style scoped>
  div {
    display: grid;
    grid-template-columns: 1fr; /* Creates one column */
    grid-template-rows: 1fr;    /* Creates one row */

  }

  div > * {
    grid-row: 1 / 2;    /* Starts at row line 1, ends before row line 2 */
    grid-column: 1 / 2; /* Starts at column line 1, ends before column line 2 */
  }
</style>
