<template>
    <footer>
        <FooterTopbar />
        <FooterContent />
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
    }
}
</script>

<style lang="scss" scoped>

</style>