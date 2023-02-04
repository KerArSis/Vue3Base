<script>
  export default{
    data(){
      
    },
    methods: {
      show: function(){
        alert(new Date());
      }
    }
  }
</script>

<template>
    <button @click="show"> text </button>
    <button @mouseenter="show"> text </button>
</template>

<style>

</style>
