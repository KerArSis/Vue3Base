<script>
export default{
data(){
return{
    isValid: true,
    isDisabled: true,
}
}
}
</script>

<template>
<p :class="{valid: isValid, disable: isDisabled}">Conclave</p>
</template>

<style>
  
</style>
