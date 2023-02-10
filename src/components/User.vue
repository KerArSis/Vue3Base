<script>
export default {
    props: ['name'],
    data() {
        return {
        }
    }
}
</script>

<template>
<ul>
    <li v-for="bmw in name">{{ bmw }}</li>
</ul>
</template>