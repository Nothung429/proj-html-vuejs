<template>
    <section class="info my-5">
        <div class="info__quickstart py-5 text-center">
            <h5>Quickstart</h5>
            <h2>Awesome isn't it? Let's dive in!</h2>
            <p>Start working with <span class="logo-name">Landrick</span> that can provide everything you need to generate awereness, drive traffic, connect</p>
            <img src="../../../assets/img/imgInfo.png" alt="">
            <p class="info__quickstart__icon">
                <i class="fa-regular fa-circle-check"></i> <span>Organize your data</span>
                <i class="fa-regular fa-circle-check"></i> <span>Work with any team</span>
            </p>
        </div>
        <div class="info__tools row">
            <div class="info__tools__text col-6">
                <h2 class="py-3">Build tools and <br> extensive documentation</h2>
                <p class="info__tools__text__description py-3">You can combine all the Landrick templates into a single one, you can take a component from the Application theme and use it in the Website.</p>
                <p class="info__tools__text__icon"><i class="fa-regular fa-circle-check"></i> <span>Digital Marketing Solutions for Tomorrow</span></p>
                <p class="info__tools__text__icon"><i class="fa-regular fa-circle-check"></i> <span>Our Talented & Experienced Marketing Agency</span></p>
                <p class="info__tools__text__icon"><i class="fa-regular fa-circle-check"></i> <span>Create your own skin to match your brand</span></p>
                <button class="my-3">Read More <i class="fa-solid fa-arrow-right"></i></button>
            </div>
            <div class="info__tools__img col-6">
                <img src="../../../assets/img/1.png" alt="info img">
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
        &__quickstart {
            h5 {
                color: #2f55d4;
            }
            img {
                border-radius: 10px;
            }
            &__icon {
                color: #2eca8b;
                span {
                    margin-right: 20px;
                    color: #000;
                }
            }
        }
        &__quickstart > * {
            margin-bottom: 20px;
        }
        &__tools {
            display: flex;
            align-items: center;
            margin: 80px 0;
            height: 500px;
            &__text {
                &__description {
                    color: #8492a6;
                }
                &__icon {
                    color: #2f55d4;
                    span {
                        color: #8492a6;
                    }
                }
                button {
                    padding: 8px 18px;
                    border-radius: 8px;
                    font-weight: 600;
                    box-shadow: 3px 3px 3px #8492a6;
                    background-color: #2f55d4;
                    color: #f8f9fc;
                    border: none;
                }
            }
            &__img {
                text-align: right;
                img {
                    max-height: 450px;
                }
            }
        }
    }
</style>