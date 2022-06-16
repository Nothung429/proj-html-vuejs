<template>
    <section class="info my-5">
        <div class="info__quickstart">
            <h5>Quickstart</h5>
            <h2>Awesome isn't it? Let's dive in!</h2>
            <p>Start working with <span class="logo-name">Landrick</span> that can provide everything you need to generate awereness, drive traffic, connect</p>
            <img src="../../../assets/img/imgInfo.png" alt="">
            <p>
                <i class="fa-regular fa-circle-check"></i> <span>Organize your data</span>
                <i class="fa-regular fa-circle-check"></i> <span>Work with any team</span>
            </p>
        </div>
        <div class="info__tools">
            <div class="info__tools__text">
                <h2>Build tools and extensive documentation</h2>
                <p>You can combine all the Landrick templates into a single one, you can take a component from the Application theme and use it in the Website.</p>
                <p><i class="fa-regular fa-circle-check"></i> Digital Marketing Solutions for Tomorrow</p>
                <p><i class="fa-regular fa-circle-check"></i> Our Talented & Experienced Marketing Agency</p>
                <p><i class="fa-regular fa-circle-check"></i> Create your own skin to match your brand</p>
                <button>Read More <i class="fa-solid fa-arrow-right"></i></button>
            </div>
            <div class="info__tools__img">
                <img src="../../../assets/img/1.png" alt="">
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "MainInfo",
    }
</script>

<style lang="scss" scoped>
    .info {
        background-color: lightseagreen;
        &__tools {
            display: flex;
            align-items: center;
            margin: 80px 0;
            height: 500px;
        }
    }
</style>