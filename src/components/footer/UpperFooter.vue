<template>
    <div class="upper-footer">
        <div class="container">
            <nav>
                <div class="menu" v-for="item in menu">
                    <ul>
                        <h3>{{item.sectionName}}</h3>
                        <li v-for="item in item.content">
                            <a :href="item.link" :target="item.target">{{item.text}}</a>
                        </li>
                    </ul>
                </div>           
            </nav>
            <FooterDCLogo/>
        </div>
    </div>
</template>

<script>
import FooterDCLogo from './FooterDCLogo.vue';
export default {
    name: 'UpperFooter',
    components: {
        FooterDCLogo,
    },
    data() {
        return {
            menu: [
                {
                    sectionName: 'dc comics',
                    content: [
                        {
                            text: 'Characters',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Comics',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Movies',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'TV',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Games',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Videos',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'News',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                },
                {
                    sectionName: 'shop',
                    content: [
                        {
                            text: 'Shop DC',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Shop DC collectibles',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                },
                {
                    sectionName: 'dc',
                    content: [
                        {
                            text: 'Characters',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Comics',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Movies',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'TV',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Games',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Videos',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'News',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'TV',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Games',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Videos',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'News',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                }, {
                    sectionName: 'sites',
                    content: [
                        {
                            text: 'Characters',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Comics',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Movies',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'TV',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Games',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                }
            ]
        }
    },
   
}
</script>

<style scoped lang="scss">
@use 'src/styles/variables.scss' as *;
        .upper-footer {
            justify-content: center;
            overflow: hidden;
            display: flex;
            width: 100%;          
            background-image: url(src/assets/img/footer-bg.jpg);
            background-repeat: no-repeat;
            background-size: cover;
            .container{
                width: 75%;
                display: flex;             
                max-height: 450px;                       
                justify-content: space-between;
                nav{
                    display: flex;
                    flex-direction: column;
                    flex-wrap: wrap;
                    font-size: 20px;
                }
                    h3{
                        color: $primary--color;
                        text-transform: uppercase;
                    }
                    li{
                        list-style-type: none;
                    }
                    a{
                        text-decoration: none;
                        color: $icon--bg-color;
                    }
                }
        }
</style>
