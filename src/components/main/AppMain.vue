<template>
    <main>
        <JumboMain/>
        <div class="ads">
            <AdsMain/>
        </div>
        
    </main>
</template>

<script>
import JumboMain from './JumboMain.vue';
import AdsMain from './AdsMain.vue';
export default {
    name: 'AppMain',
    components: {
        JumboMain,
        AdsMain,
    }
}
</script>

<style scoped lang="scss">
@use 'src/styles/variables.scss' as *;
        .ads{
            display: flex;
            justify-content: center;
            background-color: $complementary--color;
        }
</style>
