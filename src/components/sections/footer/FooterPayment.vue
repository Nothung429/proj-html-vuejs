<template>
    <div class="payment">
        <div class="payment__credits">
            <p>© 2020 Landrick. Design with ♥ by Shreethemes.</p>
        </div>
        <div class="payment__card">
            <img src="../../../assets/img/american-ex.png" alt="card info">
            <img src="../../../assets/img/discover.png" alt="card info">
            <img src="../../../assets/img/master-card.png" alt="card info">
            <img src="../../../assets/img/paypal.png" alt="card info">
            <img src="../../../assets/img/visa.png" alt="card info">
        </div>
    </div>
</template>

<script>
    export default {
        name: "FooterPayment",
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