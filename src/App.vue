<script>
export default{
data(){
return{
    text: ' ',
    conclave: ' ',
}
},
methods: {
list: function(){
}
}
}
</script>

<template>
<textarea class="text-field__input" v-model="text"></textarea>
<p>{{ text }}</p>
<br>
<button @click="Alex">Alex</button>
<ul>
<li v-for="Text in text">{{ Text }}</li>
</ul>
</template>

<style>
  
</style>
