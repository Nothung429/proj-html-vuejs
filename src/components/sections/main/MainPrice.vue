<template>
    <section class="price my_5">
        <div class="price__top text-center">
            <h2>Our rates for developer from landrick team</h2>
            <p>Start working with <span class="logo-name">Landrick</span> that can provide everything you need to generate <br> awereness, drive traffic, connect</p>
        </div>
        <div class="price__bottom row justify-content-evenly my-5">
            <div class="price__bottom__card col-4">
                <h4 class="type">Basic</h4>
                <h2>$9.00</h2>
                <p>Per Month</p>
                <p>All the basics for businesses that are just getting started.</p>
                <hr>
                <div>
                    <ul>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Full Access</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Enhanced Security</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Source Files</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>1 Domain Free</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Enhanced Enhanciation</span>
                        </li>
                    </ul>
                    <button class="try">Buy Now</button>
                    <p>*No credit card required</p>
                </div>
            </div>
            <div class="price__bottom__card col-4">
                <div class="ribbon ribbon-top-right">
                    <span>Best</span>
                </div>
                <h4 class="type">Business</h4>
                <h2>$39.00</h2>
                <p>Per Month</p>
                <p>Better for growing businesses that want more customer.</p>
                <hr>
                <div>
                    <ul>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Full Access</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Enhanced Security</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Source Files</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>1 Domain Free</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Enhanced Enhanciation</span>
                        </li>
                    </ul>
                    <button class="try">Buy Now</button>
                    <p>*No credit card required</p>
                </div>
            </div>
            <div class="price__bottom__card col-4">
                <h4 class="type">Enterprise</h4>
                <h2>$79.00</h2>
                <p>Per Month</p>
                <p>Advanced features for pros who need more customization.</p>
                <hr>
                <div>
                    <ul>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Full Access</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Enhanced Security</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Source Files</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>1 Domain Free</span>
                        </li>
                        <li>
                            <i class="fa-regular fa-circle-check"></i> <span>Enhanced Enhanciation</span>
                        </li>
                    </ul>
                    <button class="try">Buy Now</button>
                    <p>*No credit card required</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "MainPrice",
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
            &__card {
                width: 350px;
                padding: 20px;
                border: 1px solid #f4f5f6;
                border-radius: 10px;
                position: relative;
                z-index: 0;
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
                    color: #000;
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
                    padding: 8px 0;
                    background-color: #f17425;
                    color: #fff;
                    font: 700 18px/1 'Lato', sans-serif;
                    text-shadow: 0 1px 1px rgba(0,0,0,.2);
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