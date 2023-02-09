<script>
  export default{
    data(){
      return{
        visible: true,
        visible2: true,
        visible3: true,
      }
    },
    methods: {
      Alex: function() {
        this.visible = !this.visible;
      },
      Jason: function () {
        this.visible2 = !this.visible2;
      },
      Paul: function () {
        this.visible3 = !this.visible3;
      }
    }
  }
</script>

<template>
  <button @click="Alex">Alex</button>
  <p v-if="visible">Alex</p>
  <button @click="Jason">Jason</button>
  <p v-if="visible2">Jason</p>
  <button @click="Paul">Paul</button>
  <p v-if="visible3">Paul</p>
  </template>

<style>

</style>
