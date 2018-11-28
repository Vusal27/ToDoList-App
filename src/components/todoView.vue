<template lang="pug">
    div
        h1 {{$route.params.todo}}
        button(
            @click="goBack"
            ) Назад
</template>
<script>
export default {
    methods: {
        goBack() {
            this.$router.go(-1);
        }
    }
}
</script>
<style lang="scss" scoped>
    button {
        cursor: pointer;
        background: transparent;
        border: 1px solid transparent;
        border-radius: 3px;
        outline: none;
        padding: 5px 10px;
        &:hover {
            background: white;
            border: 1px solid rgba(178, 34, 34, .2);
        }
    }
</style>


