<template>
    <div class="jumbo">
        <div class="jumbo__hero">
            <div class="jumbo__hero__description">
                <p>Development</p>
                <h1>A Complete Developer Toolset</h1>
                <p>Launch your campaign and benefit from our expertise on designing and managing conversion centered bootstrap4 html page.</p>
                <button>Get started</button>
                <button>Documentation</button>
                <p>Current Version: v2.6.0</p>
            </div>
            <div class="jumbo__hero__img">
                <img src="../../../assets/img/about.png" alt="jumbo img">
            </div>
        </div>
        <div class="jumbo__partner">
            <img src="../../../assets/img/amazon.svg" alt="partner logo">
            <img src="../../../assets/img/google.svg" alt="partner logo">
            <img src="../../../assets/img/lenovo.svg" alt="partner logo">
            <img src="../../../assets/img/paypal.svg" alt="partner logo">
            <img src="../../../assets/img/shopify.svg" alt="partner logo">
            <img src="../../../assets/img/spotify.svg" alt="partner logo">
        </div>
    </div>
</template>

<script>
    export default {
        name: "HeaderJumbo",
    }
</script>

<style lang="scss" scoped>
    .jumbo {
        &__hero {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px 0;
            height: 500px;
            background-color: lightgray;
            border-bottom: 2px solid red;
            &__description {
                width: 40%;
            }
            &__img {
                width: 40%;
                object-fit: contain;
                img {
                    object-fit: contain;
                }
            }
        }
        &__partner {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 200px;
            background-color: lightgray;
            img {
                max-width: 100px;
                margin: 0 20px;
            }
        }
    }
</style>