<template>
    <section class="footer-topbar">
        <div class="buy container">
            <div class="buy-item">
                <div class="img-container">
                    <img src="../assets/buy-comics-digital-comics.png" alt="digital comics">
                </div>

                <div class="buy-text">DIGITAL COMICS</div>
            </div>
            <div class="buy-item">
                <div class="img-container">
                    <img src="../assets/buy-comics-merchandise.png" alt="merchandise">
                </div>

                <div class="buy-text">DC MERCHANDISE</div>
            </div>
            <div class="buy-item">
                <div class="img-container">
                    <img src="../assets/buy-comics-shop-locator.png" alt="subscription">
                </div>

                <div class="buy-text">SUBSCRIPTION</div>
            </div>
            <div class="buy-item">
                <div class="img-container">
                    <img src="../assets/buy-comics-subscriptions.png" alt="shop locator">
                </div>

                <div class="buy-text">COMIC SHOP LOCATOR</div>
            </div>
            <div class="buy-item">
                <div class="img-container">
                    <img src="../assets/buy-dc-power-visa.svg" alt="dc power visa">
                </div>

                <div class="buy-text">DC POWER VISA</div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterTopbar',
}
</script>

<style lang="scss" scoped>
    @import '../style/colors.scss';

    .footer-topbar {
        background-color: $color-blue;

        .buy {
            display: flex;
            justify-content: space-around;
            padding: 48px 0;

            .buy-item {
                display: flex;
                align-items: center;
    
                .img-container {
                    height: 50px;
    
                    img {
                        height: 100%;

                    }
                }

                .buy-text {
                    color: $color-white;
                    margin-left: 12px;
                }
            }
        }

    }
</style>