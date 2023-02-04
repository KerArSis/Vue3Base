<script>
  export default{
    data(){
      return{
        text: 'text',
      }
    },
    methods: {
      change: function() {
        this.text = 'ууу';
      },
      change1: function() {
        this.text = 'ааа'
      }
    }
  }
</script>

<template>
  <p> {{ text }} </p>
  <button @click="change">Text 1</button>
  <button @click="change1">Text 2</button>
</template>

<style>

</style>
