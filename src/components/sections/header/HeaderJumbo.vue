<template>
    <div class="jumbo">
        <div class="jumbo__hero">
            <div class="jumbo__hero__description">
                <p class="jumbo__hero__description__type">Development</p>
                <h1>A Complete <br> Developer Toolset</h1>
                <p class="jumbo__hero__description__text">Launch your campaign and benefit from our expertise on designing and managing conversion centered bootstrap4 html page.</p>
                <button class="jumbo__hero__description__btn1">Get started</button>
                <button class="jumbo__hero__description__btn2" @click="activation" :class="{'change' : active}">Documentation</button>
                <p class="jumbo__hero__description__version">Current Version: v2.6.0</p>
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
        data () {
            return {
                active: false,
            }
        },
        methods: {
            activation() {
                this.active = !this.active;
            },
        }
    }
</script>

<style lang="scss" scoped>
    .jumbo {
        &__hero {
            display: flex;
            align-items: center;
            margin: 80px 0;
            height: 500px;
            &__description > * {
                margin: 10px 0;
            }
            &__description {
                width: 50%;
                h1 {
                    font-size: 36px;
                }
                &__type {
                    background-color: #e4e9f8;
                    border: 1px solid #d1daf6;
                    color: #2f55d4;
                    width: 110px;
                    text-align: center;
                    border-radius: 10px;
                    font-size: 14px;
                    font-weight: 600;
                }
                &__text, &__version {
                    color: #909daf;
                }
                &__btn1, &__btn2 {
                    padding: 8px 18px;
                    border-radius: 8px;
                    font-weight: 600;
                    box-shadow: 3px 3px 3px #8492a6;
                }
                &__btn1 {
                    background-color: #2f55d4;
                    color: #f8f9fc;
                    border: none;
                    margin-right: 20px;
                }
                &__btn2 {
                    background-color: #f8f9fc;
                    color: #2f55d4;
                    border: 1px solid #2f55d4;
                }
            }
            .change {
                color: #e4e9f8;
                background-color: #2f55d4;
            }
            &__img {
                width: 50%;
                text-align: center;
            } 
        }
    }
</style>