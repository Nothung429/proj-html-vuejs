<template>
    <div class="links row py-5">
        <div class="links__social col-3 px-3">
            <div class="links__social__logo mb-3">
                <img src="../../../assets/img/logo-light.png" alt="footer logo">
            </div>
            <p>Start working with Landrick that can provide everything you need to generate awareness, drive traffic, connect.</p>
            <div class="links__social__socials">
                <ul class="d-flex">
                    <li class="mx-2" v-for="(socialLink, index) in socialLinks" :key="index" :class="{active : socialLink.current}">
                        <a :href="socialLink.url"><i :class="socialLink.icon"></i></a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="links__company col-3 px-3">
            <h4 class="mb-3">Company</h4>
            <ul>
                <li class="my-2" v-for="(companyLink, index) in companyLinks" :key="index" :class="{active : companyLink.current}">
                    <a :href="companyLink.url"><i class="me-2" :class="companyLink.icon"></i> {{companyLink.text}}</a>
                </li>
            </ul>
        </div>
        <div class="links__useful col-3 px-3">
            <h4 class="mb-3">Useful Links</h4>
            <ul>
                <li class="my-2" v-for="(usefullLink, index) in usefullLinks" :key="index" :class="{active : usefullLink.current}">
                    <a :href="usefullLink.url"><i class="me-2" :class="usefullLink.icon"></i> {{usefullLink.text}}</a>
                </li>
            </ul>
        </div>
        <div class="links__newsletter col-3 px-3">
            <h4 class="mb-3">NewsLetter</h4>
            <p>Sign up and receive the latest tips via email.</p>
            <form action="">
                <label for="input">Write your email <span class="red">*</span></label>
                <input type="text" placeholder="Your email:">
                <br>
                <button type="submit">Subscribe</button>
            </form>
        </div>
    </div>
</template>

<script>
    export default {
        name: "FooterLinks",
        data () {
            return {
                socialLinks: [
                    {
                        "icon": "fa-brands fa-facebook-f",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-brands fa-instagram",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-brands fa-twitter",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-brands fa-linkedin-in",
                        "url": "#",
                        "current": true,
                    },
                ],
                companyLinks: [
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "About us",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Services",
                        "url": "#",
                        "current": true,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Team",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Pricing",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Project",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Careers",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Blog",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Login",
                        "url": "#",
                        "current": false,
                    },
                ],
                usefullLinks: [
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Terms of Services",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Privacy Policy",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Documentation",
                        "url": "#",
                        "current": true,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Changelog",
                        "url": "#",
                        "current": false,
                    },
                    {
                        "icon": "fa-solid fa-angle-right",
                        "text": "Components",
                        "url": "#",
                        "current": false,
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .links {
        &__social, &__company, &__useful, &__newsletter {
            a {
                text-decoration: none;
                color: #a7afb8;
            }
            .active a{
                color: #2f55d4;
            }
        }
        &__social {
            &__logo {
                max-width: 120px;
            }
            &__socials li {
                height: 40px;
                width: 40px;
                line-height: 40px;
                text-align: center;
                border: 1px solid #a7afb8;
                border-radius: 10px;
                font-size: 22px;
            }
            p {
                color: #a7afb8;
            }
        }
        &__newsletter {
            color: #a7afb8;
            h4 {
                color: #fff;
            }
            form {
                input {
                    width: 100%;
                    padding: 10px 20px;
                    border-radius: 10px;
                    border: none;
                    background-color: #27314f;
                }
                button {
                    width: 100%;
                    padding: 10px 0;
                    text-align: center;
                    border-radius: 10px;
                    border: none;
                    background-color: #222e51;
                    color: #2f55d4;
                    box-shadow: 3px 3px 3px #2f55d4;
                }
            }
            form > * {
                margin: 10px 0;
            }
        }
    }
</style>