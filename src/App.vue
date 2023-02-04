<script>
  export default{
    data(){
      return{
        arr: [1, 2, 3],
        arr2: ['x', 'y', 'z'],
      }
    }
  }
</script>

<template>
  <div>
    <p> {{arr2[0]}} </p>
    <p> {{arr2[1]}} </p>
    <p> {{arr2[2]}} </p>
    {{arr[0]+ arr[1]+arr[2]}}
  </div>
</template>

<style>

</style>
