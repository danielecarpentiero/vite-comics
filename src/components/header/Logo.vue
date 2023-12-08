<template>
    <a :href="logoLink"><img :src="assets/img/dc-logo.png" alt=""></a>
</template>

<script>
export default {
    name: 'Logo',
    data () {
        return {
            logoSrc: "../../assets/img/dc-logo.png",
            logoAlt: "CD",
            logoLink: "#",
        }
    }
}
</script>

<style scoped>
    img {
        width: 10%;
    }
</style>
