<template>
    <footer>
        <FooterTopbar />
        <FooterContent 
            :footerList="footerList" 
        />
        <FooterBottombar />
    </footer>
</template>

<script>
import FooterTopbar from './FooterTopbar.vue'
import FooterContent from './FooterContent.vue'
import FooterBottombar from './FooterBottombar.vue'

export default {
    name: 'Footer',
    components: {
        FooterTopbar,
        FooterContent,
        FooterBottombar
    },
    props: {
        footerList: Array,
    },

}
</script>

<style lang="scss" scoped>

</style>