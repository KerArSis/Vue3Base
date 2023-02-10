<script>
import BMW from './components/User.vue'
export default {
data() {
    return {
    name: 'Arsen Kerimov',
    salary: '1000',
    age: '19',
    }
},
components: {
    BMW
}
}
</script>

<template>
<BMW :name="name" :salary="salary" :age="age"/>
</template>

<style>
  
</style>
