<script>
export default {
    emits: ['show', 'show1'],
    data() {
        return {
        }
    },
    methods: {
        aaa() {
            this.$emit('show','Arsen Kerimov');
        },
        bbb() {
            this.$emit('show1','Alex Bane','20000');
        },
    }
}
</script>

<template>
<button  @click="aaa">Name</button>
<button  @click="bbb">Salary</button>
</template>