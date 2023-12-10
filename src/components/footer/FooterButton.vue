<template>
    <button>{{ buttonText }}</button>
</template>

<script>
export default {
    name: 'FooterButton',
    props: {
        buttonText: 'Sign up now!'
    }
}
</script>

<style scoped lang="scss">
@use 'src/styles/variables.scss' as *;
button {
    background-color: $lighter--secondary--color;
    border: 2px solid $complementary--color;
    text-transform: uppercase;
    
}
</style>
