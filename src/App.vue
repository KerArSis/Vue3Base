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
    BMW() {
    alert('Alex, Jason, Paul');
    },
    bmw(){
    alert('Jace, Tom, Ben')
    }
}
}
</script>

<template>
<BMW @show="BMW" @show1="bmw" />
</template>

<style>
  
</style>
