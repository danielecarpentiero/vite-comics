<template>
    <header>
        <Logo/>
        <HeaderNav/>
    </header>
</template>

<script>
import Logo from './Logo.vue';
import HeaderNav from './HeaderNav.vue';
export default {
    name: 'AppHeader',
    components: {
        Logo,
        HeaderNav
    }
}
</script>

<style scoped>
    header{
        display: flex;
        width: 75%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
    }
</style>
