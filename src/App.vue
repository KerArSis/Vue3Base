<script>
export default{
data(){
return{
    languages: [],
}
}
}
</script>

<template>
<div>
<input type="checkbox" v-model="languages" value="Информатика">
<label>Информатика</label>
<br>
<input type="checkbox" v-model="languages" value="Математика">
<label>Математика</label>
<br>
<input type="checkbox" v-model="languages" value="Английский">
<label>Английский</label>
<ol>
<li v-for="elem in languages">{{ elem }}</li>
</ol>
</div>
<br>
</template>

<style>
  
</style>
