<template>
    <div class="block">
        <Text :colorT="color"/>
        <button @click="out">pressBlock</button>
    </div>
</template>

<script>
    import Text from './Text.vue' 
    export default {
        name: "Block",
        props: ['color'],
        components: {
            Text
        },
        data() {
            return {
                col: this.color
            }
        },
        methods: {
            out() {
                console.log(this.col)
            }
        },
    }
</script>

<style>
    .block {
        border: 1px solid #000;
        width: 500px;
        height: 300px;
        text-align: center;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .pinbl {
        /* color: ; */
    }
</style>