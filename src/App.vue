<script>
export default{
data(){
return{
    cssClasses: 'BMW',
    visible: true,
    style: {
    hidden: true,
}
}
},
methods: {
setDone:function(){
this.style.hidden = false;
},
setTwo: function(){
this.style.hidden = true;
},
bmw: function () {
    this.visible = !this.visible;
}
}
}
</script>

<template>
<button @click="bmw">BMW</button>
<p class="BMW" v-if="visible">BMW</p>
<p :class="style">Conclave</p>
<button @click="setDone">показывает</button>
<button @click="setTwo">прячет</button>
</template>

<style>
  
</style>
