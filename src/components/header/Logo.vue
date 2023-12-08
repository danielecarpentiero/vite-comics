<template>
    <a :href="logoLink"><img :src="logoSrc" :alt="logoAlt"></a>
</template>

<script>
export default {
    name: 'Logo',
    data () {
        return {
            logoSrc: "src/assets/img/dc-logo.png",
            logoAlt: "CD",
            logoLink: "#",
        }
    }
}
</script>

<style scoped>  
</style>
