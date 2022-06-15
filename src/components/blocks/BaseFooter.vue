<template>
    <footer>
        <div class="container">
            <FooterLinks/>
        </div>
        <hr>
        <div class="container">
            <FooterPayment/>
        </div>
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
    footer {
        background-color: #202942;
        color: #fff;
    }
</style>