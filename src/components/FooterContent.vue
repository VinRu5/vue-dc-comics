<template>
    <section class="footer-content">
        <div class="container">
            <div class="footer-list">
                <ul>
                    <li>DC COMICS</li>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">News</a></li>
                </ul>
                <ul>
                    <li>SHOP</li>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibles</a></li>
                </ul>
                <ul>
                    <li>DC</li>
                    <li><a href="#">Term Of Use</a></li>
                    <li><a href="#">Privacy policy(New)</a></li>
                    <li><a href="#">Ad Choice</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscriptions</a></li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
                <ul>
                    <li>SITES</li>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
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
                        color: $color-white;
                        font-size: 12px;
                        line-height: 1.5;

                        &:first-child {
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