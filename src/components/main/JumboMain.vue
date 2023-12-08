<template>
        <h1 class="jumbotron">Content goes here</h1>
</template>

<script>
export default {
    name: 'JumboMain',
    data() {
        return {
        };
    },   
};
</script>

<style scoped lang="scss">
@use 'src/styles/variables.scss' as *;
    .jumbotron {
        background-color: $secondary--color;
        margin: 0;
        color: $primary--color;
        padding: 60px;
        font-size: 2rem;
    }
</style>
