<script>
export default{
data(){
return{
    students: [
    {
        id: 1,
        name: 'Arsen',
        surn: 'Kerimov',
        salary: 100,
		age: 19,
    },
    {
        id: 2,
        name: 'Alex',
        surn: 'Bane',
        salary: 200,
		age: 18,
    },
    {
        id: 3,
        name: 'Jason',
        surn: 'Lightwood',
        salary: 300,
		age: 25,
    },
    ],
}
},
methods: {
edit(student) {
    student.isEdit = true;
},
save(student) {
    student.isEdit = false;
},
}
}
</script>

<template>
<table>
<tr v-for="student in students" :key="student.id"> 
<template v-if="!student.isEdit">
{{ student.name }} {{ student.surn }} {{ student.salary }} {{ student.age }}<button class="button" @click="edit(student)">изменить</button>
</template>
<template v-else>
<input v-model="student.name">
<input v-model="student.surn">
<input v-model="student.salary">
<input v-model="student.age"><button class="button" @click="save(student)">сохранить</button>
</template>
</tr>
</table>
</template>

<style>
  
</style>
