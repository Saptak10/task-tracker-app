<template>
    <button @click="onClick()"
    :style="{ background: color }" 
    class="btn" >{{ text }}</button>
</template>

<script>
export default {
    name : 'Button',
    props: {
        // text: {
        //     type: String,
        // },
        // color: {
        //     type: String,
        // }
        text: String,
        color: String,
    },
    methods: {
        onClick() {
            // console.log('click')
            this.$emit('btn-click')
        },
    }
}
</script>

<style scoped>
    /* header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    } */
</style>