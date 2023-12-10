<template>
    <div class="footer-socials">
        <h3>follow us</h3>
        <ul>
            <li v-for="item in socials">
                <a :href="item.link" :target="item.target">
                    <img :src="item.icon" :alt="item.icon">
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'FooterSocials',
    data() {
        return {
            socials: [
                {
                    icon: 'src/assets/img/footer-facebook.png',
                    link: '#',
                    target: '_blank'
                },
                {
                    icon: 'src/assets/img/footer-twitter.png',
                    link: '#',
                    target: '_blank'
                },
                {
                    icon: 'src/assets/img/footer-youtube.png',
                    link: '#',
                    target: '_blank'
                },
                {
                    icon: 'src/assets/img/footer-pinterest.png',
                    link: '#',
                    target: '_blank'
                },
                {
                    icon: 'src/assets/img/footer-periscope.png',
                    link: '#',
                    target: '_blank'
                }
            ]
        }
    }
   }
</script>

<style scoped>
    .footer-socials {
        display: flex;
        li{
            display: flex;
        }
        
    }
    h3 {
        text-transform: uppercase;
        color: #fff;
        font-size: 20px;
        margin-bottom: 20px;
    }
    li{
        list-style: none;
    }
</style>
