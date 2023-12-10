<template>
   <FooterButton/>
    <FooterSocials/>
</template>

<script>
import FooterButton from './FooterButton.vue';
import FooterSocials from './FooterSocials.vue';
export default {
    name: 'LowerFooter',
    components: {
        FooterButton,
        FooterSocials,
    },
}
</script>

<style scoped lang="scss">
@use 'src/styles/variables.scss' as *;
</style>
