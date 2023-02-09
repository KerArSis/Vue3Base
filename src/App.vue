<script>
export default{
data(){
return{
    checked: true,
    visible: true,
}
},
methods: {
BMW: function () {
    this.checked = false;
    this.visible = !this.visible;
},
}
}
</script>

<template>
<input class="text-field__input" type="checkbox" v-model="checked"> 
<button @click="BMW">BMW</button>
<p v-if="visible">{{ checked ? 'Alex' : 'Jason' }}</p>
</template>

<style>
  
</style>
