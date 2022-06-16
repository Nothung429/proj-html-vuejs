<template>
    <main>
        <div class="container">
            <MainFeatures/>
            <MainInfo/>
            <MainPrice/>
            <MainNews/>
        </div>
    </main>
</template>

<script>
    import MainFeatures from "../sections/main/MainFeatures.vue"
    import MainInfo from "../sections/main/MainInfo.vue"
    import MainPrice from "../sections/main/MainPrice.vue"
    import MainNews from "../sections/main/MainNews.vue"

    export default {
        name: "BaseMain",
        components: {
            MainFeatures,
            MainInfo,
            MainPrice,
            MainNews,
        }
    }
</script>

<style lang="scss" scoped>
    
</style>