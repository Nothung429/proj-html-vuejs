<template>
    <header>
        <div class="container">
            <HeaderNavbar/>
            <HeaderJumbo/>
        </div>
        <hr>
        <div class="container">
            <HeaderPartner/>
        </div>
    </header>
</template>

<script>
    import HeaderNavbar from "../sections/header/HeaderNavbar.vue"
    import HeaderJumbo from "../sections/header/HeaderJumbo.vue"
    import HeaderPartner from "../sections/header/HeaderPartner.vue"

    export default {
        name: "BaseHeader",
        components: {
            HeaderNavbar,
            HeaderJumbo,
            HeaderPartner,
        }
    }
</script>

<style lang="scss" scoped>
    header {
        background-color: lightgray;
        // background-color: #f8f9fc;
        clip-path: ellipse(120% 100% at 50% 0%);
    }
</style>