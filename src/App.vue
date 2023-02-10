<script>
import BMW from './components/User.vue'
export default {
data() {
    return {
    bmw: [
        {
        id: 1,
        name: 'Alex',
        salary: 1000,
        age: 19
        },
        {
        id: 2,
        name: 'Jason',
        salary: 2000,
        age: 18
        },
        {
        id: 3,
        name: 'Paul',
        salary: 3000,
        age: 25
        },
    ],
}
},
components: {
    BMW
}
}
</script>

<template>
<BMW v-for="bmw in bmws" :name="bmws.name" :salary="bmws.salary" :age="bmws.age" :key="bmws.id" />
</template>

<style>
  
</style>
