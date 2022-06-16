<template>
    <div class="payment">
        <div class="payment__credits">
            <p>© 2020 Landrick. Design with <span class="red">♥</span> by Shreethemes.</p>
        </div>
        <div class="payment__card">
            <ul class="d-flex">
                <li class="mx-2" v-for="(cardPayment, index) in cardPayments" :key="index">
                    <a :href="cardPayment.url">
                        <img :src="cardPayment.img" :alt="cardPayment.text">
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "FooterPayment",
        data () {
            return {
                cardPayments: [
                    {
                        "img": require("../../../assets/img/american-ex.png"),
                        "url": "#",
                        "text": "american express"
                    },
                    {
                        "img": require("../../../assets/img/discover.png"),
                        "url": "#",
                        "text": "discover"
                    },
                    {
                        "img": require("../../../assets/img/master-card.png"),
                        "url": "#",
                        "text": "mastercard"
                    },
                    {
                        "img": require("../../../assets/img/paypal.png"),
                        "url": "#",
                        "text": "paypal"
                    },
                    {
                        "img": require("../../../assets/img/visa.png"),
                        "url": "#",
                        "text": "visa"
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .payment {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100px;
        &__card {
            img {
                margin-left: 10px;
                border-radius: 7px;
            }
        }
    }
</style>