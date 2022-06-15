<template>
    <div class="links">
        <div class="links__social">
            <div class="links__social__logo">
                <img src="../../../assets/img/logo-light.png" alt="footer logo">
            </div>
            <p>Start working with Landrick that can provide everything you need to generate awareness, drive traffic, connect.</p>
            <div class="links__social__socials">
                <ul>
                    <li><i class="fa-brands fa-facebook-f"></i></li>
                    <li><i class="fa-brands fa-instagram"></i></li>
                    <li><i class="fa-brands fa-twitter"></i></li>
                    <li><i class="fa-brands fa-linkedin-in"></i></li>
                </ul>
            </div>
        </div>
        <div class="links__company">
            <h4>Company</h4>
            <ul>
                <li>home</li>
                <li>home</li>
                <li>home</li>
                <li>home</li>
                <li>home</li>
                <li>home</li>
                <li>home</li>
                <li>home</li>
            </ul>
        </div>
        <div class="links__useful">
            <h4>Useful Links</h4>
            <ul>
                <li>home</li>
                <li>home</li>
                <li>home</li>
                <li>home</li>
                <li>home</li>
            </ul>
        </div>
        <div class="links__newsletter">
            <h4>NewsLetter</h4>
            <p>Sign up and receive the latest tips via email.</p>
            <form action="">
                <label for="input">Write your email *</label>
                <input type="text" placeholder="Your email:">
                <button type="submit">Subscribe</button>
            </form>
        </div>
    </div>
</template>

<script>
    export default {
        name: "FooterLinks",
    }
</script>

<style lang="scss" scoped>
    .links {        
        display: flex;
        padding: 20px 0;
        &__social {
            &__logo {
                max-width: 120px;
            }
        }
    }
</style>