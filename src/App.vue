<script>
import BMW from './components/User.vue'
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
    BMW
},
methods: {
    remove(id) {
    this.bmw = this.bmw.filter((bmws) => {
        return bmws.id !== id;
    })
    }
}
}
</script>

<template>
<BMW v-for   ="bmws in bmw"
		:id     ="bmws.id"
		:name   ="bmws.name"
		:surn   ="bmws.surn"
		@remove ="remove"
		:key    ="bmws.id"/>
</template>

<style>
  
</style>
