<template>
    <header>
        <HeaderNavbar/>
        <HeaderJumbo/>
    </header>
</template>

<script>
    import HeaderNavbar from "../sections/header/HeaderNavbar.vue"
    import HeaderJumbo from "../sections/header/HeaderJumbo.vue"

    export default {
        name: "BaseHeader",
        components: {
            HeaderNavbar,
            HeaderJumbo,
        }
    }
</script>

<style lang="scss" scoped>

</style>