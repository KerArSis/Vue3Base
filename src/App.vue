<script>
import BMW from './components/User.vue'
import UserForm from './components/UserForm.vue'
export default {
data() {
    return {
    bmw: [
        {
        id: 1,
        name: 'Alex',
        surn: 'BMW'
        },
        {
        id: 2,
        name: 'Jason',
        surn: 'BMW'
        },
        {
        id: 3,
        name: 'Paul',
        surn: 'BMW'
        },
    ],
    }
},
components: {
    BMW, UserForm
},
methods: {
    add(name, surn){
    let id = this.bmw.length + 1;
    this.bmw.push({
        id, name, surn
    });
    }
}
}
</script>

<template>
<UserForm @add="add"/>
</template>

<style>
  
</style>
