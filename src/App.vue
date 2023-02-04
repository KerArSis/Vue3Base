<script>
  export default{
    data(){
      return{
      }
    },
    methods: {
      show: function(str){
        alert(str*str);
      },
      show1: function(str1){
        alert(str1*str1)
      }
    }
  }
</script>

<template>
  <button @click="show(2)">квадрат числа 2</button>
  <button @click="show1(3)">квадрат числа 3</button>
</template>

<style>

</style>
