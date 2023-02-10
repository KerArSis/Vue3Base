<script>
export default {
    emits: ['show'],
    data() {
        return {
        }
    },
    methods: {
    }
}
</script>

<template>
<button @click="$emit('show', 'Arsen Kerimov')">Name</button>
</template>