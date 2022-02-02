<template>
    <p :style="{color: colorT}" class="text">Text Should change color!</p>
    <button @click="log">PressText</button>
</template>
<script>
    export default {
        name: 'Text',
        props: ['colorT'],
        data() {
            return {
                colorr: this.colorT
            }
        },
        methods: {
            log() {
                console.log(this.colorr)
            }
        },
    }
</script>
<style>
</style>