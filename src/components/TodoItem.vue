<template>
    <li class="item" @click="handleClick">{{content}}</li>
</template>

<script>
export default {
    props: ["content", "index"],
    methods: {
        handleClick () {
            this.$emit("delete", this.index);
        }
    }
}
</script>

<style lang="scss" scoped>
    .item {
        color: #f00;
    }
</style>
