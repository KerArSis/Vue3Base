<script>
  export default{
    data(){
      return{
        obj: {a:'100$', b:'200$', c:'300$'},
      }
    }
  }
</script>
<template>
<ul>
    <li v-for="elem in obj">{{ elem }}</li>
</ul>
<br>
<br>
<ul>
    <li v-for="(key, elem) in obj"> {{ elem }} - {{ key }}</li>
</ul>
<br>
<br>
<ul>
    <li v-for="(key, elem, index) in obj"> {{ elem }} - {{ key }} - {{ index }}</li>
</ul>
<br>
<br>
<ul>
    <li v-for="(key, elem, index) in isSmeshariki"> {{ elem }} - {{ key }} - {{ index+1 }}</li>
</ul>
</template>

<style>

</style>
