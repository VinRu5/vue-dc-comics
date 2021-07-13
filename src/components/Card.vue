<template>
    <div class="card-container">
        <div class="img-container">
            <img :src="thumb" alt="">
        </div>
        <div class="title">{{ upperTitle }}</div>
        <div class="price">{{ price }}</div>
        <div class="type">{{ type }}</div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        thumb: String,
        title: String,
        price: String,
        type: String,
    },
    computed: {
        upperTitle: function() {
            return this.title.toUpperCase();
        }
    }
}
</script>

<style lang="scss" scoped>

    .card-container {
        margin-bottom: 24px;
        flex-basis: calc(100% / 6);

        .img-container {
            width: 100%;
            height: calc(1200px / 6);
            overflow: hidden;
            margin-bottom: 12px;

           .img {
               width: 100%;
           }
        }
    }

</style>