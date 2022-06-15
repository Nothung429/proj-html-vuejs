
<template>
    <div id="app">
        <div class="container">
            <BaseHeader/>
            <BaseMain/>
            <BaseFooter/>
        </div>
    </div>
</template>

<script>
    import BaseHeader from "./components/blocks/BaseHeader.vue"
    import BaseMain from "./components/blocks/BaseMain.vue"
    import BaseFooter from "./components/blocks/BaseFooter.vue"
        
    export default {
        name: "App",
        components: {
            BaseHeader,
            BaseMain,
            BaseFooter,
        }
    }
</script>

<style lang="scss">
    @import "assets/style/general.scss";
</style>