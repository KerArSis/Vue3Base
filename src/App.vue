<script>
  export default {
    data() {
      return {
        visible1: true,
        visible2: false,
      }
    },
  }
</script>

<template>
  <div v-if="visible1">True</div>
  <div v-if="!visible2">False</div>
</template>

<style>

</style>
