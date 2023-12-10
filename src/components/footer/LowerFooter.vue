<template>
    <footer>
        <div class="container">
            <FooterButton/>
             <FooterSocials/>
        </div>
    </footer>
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
footer {
    background-color: $lighter--secondary--color;
    width: 100%;
    
    .container{
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 75%;
            display: flex;
            flex-direction: column;
        }
}
</style>
