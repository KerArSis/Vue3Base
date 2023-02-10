<script>
import BMW from './components/User.vue'
export default {
data() {
    return {
    
    }
},
components: {
    BMW
},
methods: {
    aaa(name) {
    console.log(name);
    },
    bbb(name, salary){
console.log(name, salary);
    }
}
}
</script>

<template>
<BMW @show="aaa" @show1="bbb"/>
</template>

<style>
  
</style>
