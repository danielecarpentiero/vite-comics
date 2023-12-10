<template>
    <button>{{ buttonText }}</button>
</template>

<script>
export default {
    name: 'FooterButton',
    data() {
        return {
            buttonText: 'sign up now!',
        };
    },
}
</script>

<style scoped lang="scss">
@use 'src/styles/variables.scss' as *;
    button {
    background-color: $lighter--secondary--color;
    border: 2px solid $complementary--color;
    text-transform: uppercase;
    color: $complementary--color;
    }
</style>
