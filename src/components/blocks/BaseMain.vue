<template>
    <main>
        <MainFeatures/>
        <MainInfo/>
        <MainPrice/>
    </main>
</template>

<script>
    import MainFeatures from "../sections/main/MainFeatures.vue"
    import MainInfo from "../sections/main/MainInfo.vue"
    import MainPrice from "../sections/main/MainPrice.vue"

    export default {
        name: "BaseMain",
        components: {
            MainFeatures,
            MainInfo,
            MainPrice,
        }
    }
</script>

<style lang="scss" scoped>

</style>