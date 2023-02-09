<script>
  export default {
    data() {
      return {
        bmw: true,
      }
    },
    methods: {
      BMW: function() {
        this.bmw = false;
      }
    }
  }
</script>

<template>
  <button @click="BMW">BMW</button>
  <div v-if="bmw">
  <p>Alex</p>
  <p>Jason</p>
  <p>Paul</p>
  </div>
</template>

<style>

</style>
