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
    bmwName(name) {
    console.log(name);
    },
}
}
</script>

<template>
<BMW @show="bmwName"/>
</template>

<style>
  
</style>
