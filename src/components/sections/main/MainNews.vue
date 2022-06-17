<template>
    <section class="news my-5">
        <h2 class="pt-3">Want to be among the first to find out?</h2>
        <p class="pb-3">Start working with <span class="logo-name">Landrick</span> that can provide everything you need to generate awereness, drive traffic, connect</p>
        <input type="text" placeholder="Email Address">
        <button class="start">Get Started</button>
    </section>
</template>

<script>
    export default {
        name: "MainPrice",
    }
</script>

<style lang="scss" scoped>
    .news {
        position: relative;
        text-align: center;
        input {
            width: 50%;
            border-radius: 30px;
            border: 1px solid #000;
            padding: 10px 20px;            
        }
        .start {
            position: absolute;
            top: 124px;
            right: 337px;
            border-radius: 30px;
            padding: 5px 10px;
            box-shadow: 3px 3px 3px #8492a6;
            background-color: #2f55d4;
            color: #f8f9fc;
            border: none;
        }        
    }
</style>