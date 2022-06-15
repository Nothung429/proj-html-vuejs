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
            <button><i class="fa-solid fa-magnifying-glass"></i></button>
            <button><i class="fa-brands fa-github"></i></button>
            <button><i class="fa-brands fa-stack-overflow"></i></button>
            <button><i class="fa-regular fa-user"></i></button>
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
        background-color: lightgreen;
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
            button {
                font-size: 36px;
            }
        }
    }
</style>