<template>
    <p :style="{color: colorT}" class="text">Text Should change color!</p>
</template>
<script>
    export default {
        name: 'Text',
        props: ['colorT'],
        data() {
            return {
                colorr: this.colorT
            }
        }
    }
</script>
<style>
</style>