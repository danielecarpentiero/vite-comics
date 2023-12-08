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
    
<style scoped lang="scss">

 @use "../../styles/variables.scss" as *;

    ul {
        display: flex;
        justify-content: center;
        text-transform: uppercase;
        height: 100%;
        li  {
            display: block;
            list-style: none;
            padding: 0 1.875rem;
            line-height: 100px;
            &:hover {
                border-bottom: 5px solid $complementary--color;     
            }}
    };
</style>
