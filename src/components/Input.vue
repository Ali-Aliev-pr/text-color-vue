<template>
    <input type="text" v-model="colorValue"/>
    <button @click="colorChange">Press!</button>
</template>
<script>
    export default {
        name: "Inputs",
        props: ['colorChanged'],
        data() {
            return {
                colorValue: ''
            }
        },
        methods: {
            colorChange() {
                this.colorChanged(this.colorValue)
                console.log(this.colorValue)
                this.colorValue = ''
            }
        },
    }
</script>
<style>
    
</style>