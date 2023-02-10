<script>
export default{
data(){
return{
    isDisabled: true,
    isDisabled1: true,
    checked: false,
}
},
methods: {
BMW: function () {
    this.isDisabled = false;
},
bmw: function () {
    this.isDisabled1 = false;
},
}
}
</script>
<template>
<input type="text" class="text-field__input"  v-bind:disabled="isDisabled">
<br>
<button @click="BMW">BMW</button>
<br>
<br>
<br>
<input type="text" class="text-field__input" v-bind:disabled="isDisabled1">
<br>
<input type="checkbox" v-model="checked" @click="bmw">
<button @click="BMW">BMW</button> 
</template>

<style>
  
</style>
