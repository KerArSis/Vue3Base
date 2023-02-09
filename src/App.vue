<script>
  export default{
    data(){
      return{
        isAuth: false,
      }
    }
  }
</script>
<template>
  <p v-if="isAuth">+++</p>
  <p v-else>---</p>
</template>

<style>

</style>
