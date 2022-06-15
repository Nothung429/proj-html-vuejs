<template>
    <div class="partner">
        <img src="../../../assets/img/amazon.svg" alt="partner logo">
        <img src="../../../assets/img/google.svg" alt="partner logo">
        <img src="../../../assets/img/lenovo.svg" alt="partner logo">
        <img src="../../../assets/img/paypal.svg" alt="partner logo">
        <img src="../../../assets/img/shopify.svg" alt="partner logo">
        <img src="../../../assets/img/spotify.svg" alt="partner logo">
    </div>
</template>

<script>
    export default {
        name: "HeaderPartner",
    }
</script>

<style lang="scss" scoped>
    .partner {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 200px;
        img {
            max-width: 100px;
            margin: 0 20px;
        }
    }
</style>