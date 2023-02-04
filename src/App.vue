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
    {{ show() }}
</template>

<style>

</style>
