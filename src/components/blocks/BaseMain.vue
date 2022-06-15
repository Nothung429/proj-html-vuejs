<template>
    <main>
        <h2>content go here</h2>
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
    main {
        height: 300px;
        background-color: lightcoral;
    }
</style>