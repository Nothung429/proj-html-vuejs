<template>
    <footer>
        <FooterLinks/>
        <FooterPayment/>
    </footer>
</template>

<script>
    import FooterLinks from "../sections/footer/FooterLinks.vue"
    import FooterPayment from "../sections/footer/FooterPayment.vue"

    export default {
        name: "BaseFooter",
        components: {
            FooterLinks,
            FooterPayment,            
        }
    }
</script>

<style lang="scss" scoped>

</style>