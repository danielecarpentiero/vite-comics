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

<style scoped lang="scss">
    header{
        display: flex;
        align-items: center;
        width: 75%;
        margin: 0 auto;
        justify-content: space-between;
        height: 120px;
    }
</style>
