<script>
  export default {
    data() {
      return {
        hidden1: true,
        hidden2: false,
      }
    },
  }
</script>

<template>
  <div v-if="hidden1">True</div>
  <div v-if="!hidden2">False</div>
</template>

<style>

</style>
