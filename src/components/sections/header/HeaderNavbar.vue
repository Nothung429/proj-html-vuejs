<template>
    <div class="navbar">
        <div class="navbar__logo">
            <img src="../../../assets/img/logo-dark.png" alt="header logo">
        </div>
        <div class="navbar__links">
            <ul>
                <li>home</li>
                <li>home</li>
                <li>home</li>
                <li>home</li>
            </ul>
        </div>
        <div class="navbar__buttons">
            <button class="navbar__buttons__search"><i class="fa-solid fa-magnifying-glass"></i></button>
            <button class="navbar__buttons__account"><i class="fa-brands fa-github"></i></button>
            <button class="navbar__buttons__account"><i class="fa-brands fa-stack-overflow"></i></button>
            <button class="navbar__buttons__account"><i class="fa-regular fa-user"></i></button>
        </div>
    </div>
</template>

<script>
    export default {
        name: "HeaderNavbar",
    }
</script>

<style lang="scss" scoped>
    .navbar {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100px;
        &__logo {
            max-width: 180px;
        }
        &__links {
            ul {
                display: flex;
                li {
                    padding: 0 15px;
                }
            }
        }
        &__buttons {
            &__search, &__account {
                font-size: 20px;
                height: 40px;
                width: 40px;
                line-height: 40px;
                text-align: center;
                border-radius: 8px;
                margin-left: 10px;
                box-shadow: 3px 3px 3px #8492a6;
            }
            &__search {
                color: #8492a6;
                background-color: #f8f9fc;
                border: none;
            }
            &__account {
                color: #2f55d4;
                background-color: #e4e9f8;
                border: 1px solid #d1daf6;
            }
        }
    }
</style>