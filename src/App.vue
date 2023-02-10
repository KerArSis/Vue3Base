<script>
export default{
data(){
return{
    bmw: '',
    BMW: ['Alex', 'Jason', 'Paul'],
}
},
methods: {
addBMW: function () {
    this.BMW.unshift(this.bmw);
}
}
}
</script>

<template>
<ul class="styled">
<li v-for="(item, index) in 
			BMW" :key="index">
    {{ item }}
</li>
</ul>
<input class="text-field__input" v-model="bmw">
<br>
<button @click="addBMW">add</button>
</template>

<style>
  
</style>
