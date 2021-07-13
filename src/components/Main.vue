<template>
    <main>
        <div class="container">
            <Card v-for="(element, index) in comics" 
                :key="index"
                :title="element.series"
                :thumb="element.thumb"
                :price="element.price"
                :type="element.type"
            />
        
        </div>
    </main>
</template>

<script>
import Card from './Card.vue'

export default {
    name: 'Main',
    components: {
        Card,
    },
    props: {
        comics: Array,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/colors.scss';

    main {
        background: $color-black;
        color: $color-white;
        font-size: 12px;
        padding: 50px 0;
        
        .container {
            display: flex;
            flex-wrap: wrap;
        }
    }
</style>