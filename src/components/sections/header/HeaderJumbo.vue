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
    }
</style>