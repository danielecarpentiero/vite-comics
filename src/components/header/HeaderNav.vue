<template>
   <ul>
    <li v-for="item in items">{{ item.name }}</li>
   </ul>
</template>

<script>
export default {
    name: 'HeaderNav',
    data() {
        return {
            items: [
                {name: 'characters', url: '#'},
                {name: 'comics', url: '#'},
                {name: 'movies', url: '#'},
                {name: 'tv', url: '#'},
                {name: 'games', url: '#'},
                {name: 'collectibles', url: '#'},
                {name: 'videos', url: '#'},
                {name: 'fans', url: '#'},
                {name: 'news', url: '#'},
                {name: 'shop', url: '#'},
            ]
        }
    },
}
</script>
    
<style scoped>
    ul li {
        list-style: none;
    }
</style>
