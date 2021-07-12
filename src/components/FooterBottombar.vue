<template>
    <section class="footer-bottombar">
        <div class="container">
            <div class="sign-up">
                SIGN-UP NOW!
            </div>
            <div class="follow-us">
                <div class="follow-text">FOLLOW US</div>
                <div class="follow-item">
                    <img src="../assets/footer-facebook.png" alt="facebook">
                </div>
                <div class="follow-item">
                    <img src="../assets/footer-twitter.png" alt="twitter">
                </div>
                <div class="follow-item">
                    <img src="../assets/footer-youtube.png" alt="youtube">
                </div>
                <div class="follow-item">
                    <img src="../assets/footer-pinterest.png" alt="pinterest">
                </div>
                <div class="follow-item">
                    <img src="../assets/footer-periscope.png" alt="periscope">
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterBottombar',
}
</script>

<style lang="scss" scoped>
    @import '../style/colors.scss';

    .footer-bottombar {
        background-color: $color-ligth-black;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 48px 0;

            .sign-up {
                color: $color-white;
                font-size: 20px;
                font-weight: 500;
                border: 2px solid $color-blue;
                padding: 12px;

            }

            .follow-us {
                display: flex;
                align-items: center;

                .follow-text {
                    font-size: 26px;
                    color: $color-blue;
                    font-weight: bold;
                }

                .follow-item {
                    margin-left: 12px;
                }
            }
        }

    }

</style>