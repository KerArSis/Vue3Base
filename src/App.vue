<script>
export default{
data(){
  return{
    language: '',
    visible: false,
    visible1: false,
    visible2: false,
  }
},
methods: {
one(){
      this.visible = true;
},
  two() {
    this.visible1 = true;
  },
  three() {
    this.visible2 = true;
  }
}
}
</script>

<template>
<div class="hunter">
<p>Какой язык ваш родной?</p>
<input name="radio" type="radio" v-model="language" value="Крымскотатарский" @click="one">
<label for="">Крымскотатарский</label>
<br>
<input name="radio" type="radio" v-model="language" value="Русский" @click="two">
<label for="">Русский</label>
<br>
<input name="radio" type="radio" v-model="language" value="Испанский" @click="three">
<label for="">Испанский</label>
</div>
<p v-if="visible">Хош кельдинъиз</p>
<p v-else-if="visible1">Добро пожаловать</p>
<p v-else-if="visible2">Bienvenido</p>
<p v-else=''> </p>

<p>Ваш выбор: {{ language }}</p>
<br>
</template>

<style>
  
</style>
