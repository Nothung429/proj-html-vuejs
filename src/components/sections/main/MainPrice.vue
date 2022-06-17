<template>
    <section class="price my_5">
        <div class="price__top text-center">
            <h2>Our rates for developer from landrick team</h2>
            <p>Start working with <span class="logo-name">Landrick</span> that can provide everything you need to generate <br> awereness, drive traffic, connect</p>
        </div>
        <div class="price__bottom row justify-content-evenly my-5">
            <div class="price__bottom__card col-3" @mouseover="hovered1 = true" @mouseleave="hovered1 = false" :class="{'grow': hovered1}">
                <h4 class="type">Basic</h4>
                <h2>$9.00</h2>
                <p>Per Month</p>
                <p>All the basics for businesses that are just getting started.</p>
                <hr>
                <ul>
                    <li class="my-2" v-for="(priceAdvantage, index) in priceAdvantages" :key="index">
                        <i :class="priceAdvantage.icon"></i> <span class="ms-2">{{priceAdvantage.text}}</span>
                    </li>
                </ul>
                <button class="try">Buy Now</button>
                <p>*No credit card required</p>
            </div>
            <div class="price__bottom__card col-3" @mouseover="hovered2 = true" @mouseleave="hovered2 = false" :class="{'grow': hovered2}">
                <div class="ribbon ribbon-top-right">
                    <span>Best</span>
                </div>
                <h4 class="type">Business</h4>
                <h2>$39.00</h2>
                <p>Per Month</p>
                <p>Better for growing businesses that want more customer.</p>
                <hr>
                <ul>
                    <li class="my-2" v-for="(priceAdvantage, index) in priceAdvantages" :key="index">
                        <i :class="priceAdvantage.icon"></i> <span class="ms-2">{{priceAdvantage.text}}</span>
                    </li>
                </ul>
                <button class="try">Buy Now</button>
                <p>*No credit card required</p>
            </div>
            <div class="price__bottom__card col-3" @mouseover="hovered3 = true" @mouseleave="hovered3 = false" :class="{'grow': hovered3}">
                <h4 class="type">Enterprise</h4>
                <h2>$79.00</h2>
                <p>Per Month</p>
                <p>Advanced features for pros who need more customization.</p>
                <hr>
                <ul>
                    <li class="my-2" v-for="(priceAdvantage, index) in priceAdvantages" :key="index">
                        <i :class="priceAdvantage.icon"></i> <span class="ms-2">{{priceAdvantage.text}}</span>
                    </li>
                </ul>
                <button class="try">Buy Now</button>
                <p>*No credit card required</p>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "MainPrice",
        data () {
            return {
                hovered1: false,
                hovered2: false,
                hovered3: false,
                priceAdvantages: [
                    {
                        "icon": "fa-regular fa-circle-check",
                        "text": "Full Access",
                    },
                    {
                        "icon": "fa-regular fa-circle-check",
                        "text": "Enhanced Security",
                    },
                    {
                        "icon": "fa-regular fa-circle-check",
                        "text": "Source Files",
                    },
                    {
                        "icon": "fa-regular fa-circle-check",
                        "text": "1 Domain Free",
                    },
                    {
                        "icon": "fa-regular fa-circle-check",
                        "text": "Enhanced Enhanciation",
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .price {
        &__top {
            p {
                color: #8492a6;
            }
        }
        &__bottom {
            &__card > * {
                margin-bottom: 20px;
            }
            .grow { 
                transition: all .2s ease-in-out;
                transform: scale(1.1);
                box-shadow: 0 5px 5px -3px #2f55d4;
            }
            &__card {
                padding: 20px;
                border: 1px solid #f4f5f6;
                border-radius: 10px;
                position: relative;
                z-index: 0;
                box-shadow: 0 5px 5px -3px gray;
                color: #8492a6;
                .try {
                    padding: 8px 18px;
                    width: 100%;
                    border-radius: 8px;
                    font-weight: 600;
                    box-shadow: 3px 3px 3px #8492a6;
                    background-color: #2f55d4;
                    color: #f8f9fc;
                    border: none;
                }
                .type {
                    background-color: #e4e9f8;
                    border: 1px solid #d1daf6;
                    color: #2f55d4;
                    text-align: center;
                    width: 50%;
                    padding: 8px;
                    border-radius: 30px;
                    font-weight: 600;
                    font-size: 18px;
                }
                h2 {
                    color: #000;
                    font-size: 36px;
                    font-weight: 700;
                }
                ul li {
                    color: #2f55d4;
                }
                ul li span {
                    color: #8492a6;
                }

                .ribbon {
                    width: 150px;
                    height: 150px;
                    overflow: hidden;
                    position: absolute;
                }
                .ribbon::before ,.ribbon::after {
                    position: absolute;
                    z-index: -1;
                    content: '';
                    display: block;
                    border: 5px solid #f17425;
                }
                .ribbon span {
                    position: absolute;
                    display: block;
                    width: 225px;
                    padding: 5px 0;
                    background-color: #f17425;
                    color: #fff;
                    text-align: center;
                }
                .ribbon-top-right {
                    top: -10px;
                    right: -10px;
                }
                .ribbon-top-right::before ,.ribbon-top-right::after {
                    border-top-color: transparent;
                    border-right-color: transparent;
                }
                .ribbon-top-right::before {
                    top: 0;
                    left: 17px;
                }
                .ribbon-top-right::after {
                    bottom: 17px;
                    right: 0;
                }
                .ribbon-top-right span {
                    left: -25px;
                    top: 30px;
                    transform: rotate(45deg);
                }
            }
            
        }
    }
</style>