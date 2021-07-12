<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="logo dc comics">
            </div>

            <nav>
                <ul>
                    <li><a href="#">CHARACTERS</a></li>
                    <li><a href="#">COMICS</a></li>
                    <li><a href="#">MOVIES</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">GAMES</a></li>
                    <li><a href="#">COLLECTIBLES</a></li>
                    <li><a href="#">VIDEOS</a></li>
                    <li><a href="#">FANS</a></li>
                    <li><a href="#">NEWS</a></li>
                    <li><a href="#">SHOP</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Navbar',
}
</script>

<style lang="scss" scoped>
    @import '../style/colors.scss';

    header .container {
        display: flex;
        justify-content: space-between;
        align-items: center;


        nav {

            ul {
                display: flex;

                li {
                    font-size: 14px;
                    font-weight: 600;
                    margin-left: 18px;
                    height: 140px;
                    line-height: 140px;
        
                    a {
                        text-decoration: none;
                        color: $color-ligth-black;

        
                        &:hover {
                            border-bottom: 6px solid $color-blue; //da sistemare
                            color: $color-blue;
                        }
                    }
                }
            }
        }
    }
</style>