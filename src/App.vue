<script>
export default{
data(){
  return{
    sity: 'Симферополь',
  }
},
methods: {
}
}
</script>

<template>
  <p>В каком городе вы живете?</p>
    <select v-model="sity">
      <option>Симферополь</option>
      <option>Бахчисарай</option>
      <option>Керчь</option>
    </select>
    <p>{{ sity }}</p>
</template>

<style>
  
</style>
