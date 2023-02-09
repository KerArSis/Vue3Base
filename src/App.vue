<script>
  export default{
    data(){
      return{
        isAuth: true,
      }
    },
    methods: {
      BMW: function(){
        this.isAuth = false;
      }
    }
  }
</script>
<template>
  <button @click="BMW">BMW</button>
  <p v-show="isAuth">text</p>
</template>

<style>

</style>
