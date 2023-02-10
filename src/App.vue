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
        name: 'ALex',
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
removeStudents: function (id) {
    this.students = this.students.filter((student) => {
    return student.id !== id;
    })
}
}
}
</script>

<template>
<table>
<tr v-for="student in students" :key="student.id"> {{ student.name }} {{ student.surn }} {{ student.salary }} {{ student.age }} <button class="button" @click="removeStudents(students.id)">remove</button>
</tr>
</table>
</template>

<style>
  
</style>
