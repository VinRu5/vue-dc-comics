<template>
    <section class="footer-content">
        <div class="container">
            <div class="footer-list">
                <ul>
                    
                    <li v-for="link in footerList[0]" :key="link.id"><a :href="link.href">{{ link.name }}</a></li>
                    
                </ul>
                <ul>
                    <li v-for="link in footerList[1]" :key="link.id"><a :href="link.href">{{ link.name }}</a></li>
                </ul>
                <ul>
                    <li v-for="link in footerList[2]" :key="link.id"><a :href="link.href">{{ link.name }}</a></li>
                </ul>
                <ul>
                    <li v-for="link in footerList[3]" :key="link.id"><a :href="link.href">{{ link.name }}</a></li>
                </ul>
            </div>
            <div class="footer-img">
                <!-- <img src="../assets/dc-logo-bg.png" alt="logo dc"> -->
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterContent',
    props: {
        footerList: Array,
    },

}
</script>

<style lang="scss" scoped>
    @import '../style/colors.scss';

    .footer-content {
        background-image: url('../assets/footer-bg.jpg');
        // overflow: hidden;

        .container {
            height: 350px;
            display: flex;
            justify-content: space-between;

            .footer-img {
                height: 100%;
                flex-basis: 50%;
                background-image: url('../assets/dc-logo-bg.png');
                background-repeat: no-repeat;
                background-position-y: center;
            }

            .footer-list {
                flex-basis: 35%;
                display: flex;
                flex-direction: column;
                flex-wrap: wrap;
                justify-content: space-between;
                padding: 48px 0;
                

                ul {
                    flex-grow: 1;
                    
                    li {
                        font-size: 12px;
                        line-height: 1.5;

                        &:first-child {
                            color: $color-white;
                            font-size: 20px;
                            font-weight: bold;
                        }

                        a {
                            color: $color-grey;
                            text-decoration: none;
                        }
                    }

                }
            }
        }
    }
</style>