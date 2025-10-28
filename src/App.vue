<template>
  <BackgroundImageCursorMask :imageSrc="imageSrc"/>
</template>

<script>
import BackgroundImageCursorMask from './components/BackgroundImageCursorMask.vue';

  export default {
    components: { BackgroundImageCursorMask },
    data() {
      return {
        imageSrc: "https://plus.unsplash.com/premium_photo-1709893398485-f9cc26bd5165?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=1632"
      }
    }
  }
</script>

<style scoped>

</style>
