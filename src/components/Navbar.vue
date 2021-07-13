<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="logo dc comics">
            </div>

            <nav>
                <ul>
                    <li v-for="item in navList" :key="item.id"><a href="#">{{ item.name }}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Navbar',
    props: {
        navList: Array,
    }
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
                        height: 100%;
                        display: inline-block;
                        text-decoration: none;
                        color: $color-ligth-black;

        
                        &:hover {
                            border-bottom: 6px solid $color-blue;
                            color: $color-blue;
                        }
                    }
                }
            }
        }
    }
</style>