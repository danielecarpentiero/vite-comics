<template>
<AppHeader/>
<AppMain/>
<AppFooter/>
</template>

<script>
import AppHeader from './components/header/AppHeader.vue';
import AppFooter from './components/footer/AppFooter.vue';
import AppMain from './components/main/AppMain.vue';
export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    AppMain
  }
}
</script>

<style>
body{
  margin: 0;
  padding: 0;
  font-family: sans-serif;
  font-family: 'Asap Condensed', sans-serif;;
}
</style>
