<script>
  export default{
    data(){
      return{
        cssClasses: 'BMW',
        obj: {
          done: true,
          selected: false,
        },
      }
    },
  }
</script>
<template>
  <p :class="selected">BMW</p>
  <p :class="obj">Alex</p>
</template>

<style>
  
</style>
