<script>
export default{
data(){
return{
    bmw: '',
    BMW: ['Alex', 'Jason', 'Paul'],
}
},
methods: {
removeBMW: function (index) {
    this.BMW.splice(index, 1);
}
}
}
</script>

<template>
<ul>
<li v-for="(item, index) in 
			BMW" :key="index">
    {{ item }}
    <br>
    <button @click="removeBMW(index)">remove</button>
</li>
</ul>
</template>

<style>
  
</style>
