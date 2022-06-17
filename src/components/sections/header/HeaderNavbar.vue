<template>
    <div class="navbar">
        <div class="navbar__logo">
            <img src="../../../assets/img/logo-dark.png" alt="header logo">
        </div>
        <div class="navbar__links">
            <ul>
                <li v-for="(headerLink, index) in headerLinks" :key="index" :class="{active : headerLink.current}">
                    <a :href="headerLink.url"><i :class="headerLink.icon"></i> {{headerLink.text}}</a>
                </li>
            </ul>
        </div>
        <div class="navbar__buttons">
            <button class="navbar__buttons__search"><i class="fa-solid fa-magnifying-glass"></i></button>
            <button class="navbar__buttons__account" @click="activation1" :class="{'change' : active1}"><i class="fa-brands fa-github"></i></button>
            <button class="navbar__buttons__account" @click="activation2" :class="{'change' : active2}"><i class="fa-brands fa-stack-overflow"></i></button>
            <button class="navbar__buttons__account" @click="activation3" :class="{'change' : active3}"><i class="fa-regular fa-user"></i></button>
        </div>
    </div>
</template>

<script>
    export default {
        name: "HeaderNavbar",
        data () {
            return {
                active1: false,
                active2: false,
                active3: false,
                headerLinks: [
                    {
                        "icon": "",
                        "text": "Home",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-chevron-down",
                        "text": "Landing",
                        "url": "#",
                        "current": true,
                    },
                    {
                        "icon": "fa-solid fa-chevron-down",
                        "text": "Pages",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-chevron-down",
                        "text": "Docs",
                        "url": "#",
                        "current": false,
                    },
                ]
            }
        },
        methods: {
            activation1() {
                this.active1 = !this.active1;
            },
            activation2() {
                this.active2 = !this.active2;
            },
            activation3() {
                this.active3 = !this.active3;
            }
        }
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
                    a {
                        text-decoration: none;
                        font-weight: 600;
                        color: #000;
                    }
                }
                .active a{
                    color: #2f55d4;
                }
            }
        }
        &__buttons {
            .change {
                color: #e4e9f8;
                background-color: #2f55d4;
            }
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