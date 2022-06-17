<template>
    <section class="features my-5">
        <div class="features__top pt-5">
            <h3>Key Features</h3>
            <p>Start working with <span class="logo-name">Landrick</span> that can provide everything you need to generate <br> awereness, drive traffic, connect</p>
        </div>
        <div class="features__bottom py-5">
            <ul class="d-flex row">
                <li class="col-3 features__bottom__card" v-for="(feature, index) in features" :key="index" @mouseover="hovered = true" @mouseleave="hovered = false" :class="{'going-up': hovered}">
                    <div><i :class="feature.icon"></i></div>
                    <h5>{{feature.title}}</h5>
                    <p>{{feature.text}}</p>
                    <a :href="feature.url">{{feature.link}}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
    export default {
        name: "MainFeatures",
        data () {
            return {
                hovered: false,
                features: [
                    {
                        "icon": "fa-solid fa-layer-group",
                        "link": "Read More >",
                        "url": "#",
                        "title": "Modular",
                        "text": "Composed in a pseudo-Latin language which more or less corresponds",                        
                    },
                    {
                        "icon": "fa-solid fa-display",
                        "link": "Read More >",
                        "url": "#",
                        "title": "Responsive",
                        "text": "Composed in a pseudo-Latin language which more or less corresponds",                        
                    },
                    {
                        "icon": "fa-solid fa-paintbrush",
                        "link": "Read More >",
                        "url": "#",
                        "title": "Customizable",
                        "text": "Composed in a pseudo-Latin language which more or less corresponds",                        
                    },
                    {
                        "icon": "fa-solid fa-minimize",
                        "link": "Read More >",
                        "url": "#",
                        "title": "Scalable",
                        "text": "Composed in a pseudo-Latin language which more or less corresponds",                        
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .features {
        &__bottom {
            ul {
                max-width: 1320px;
                margin: 0;
                justify-content: space-between;
            }
            &__card {
                width: 300px;
                padding: 20px;
                border: 1px solid #f4f5f6;
                border-radius: 5px;
                position: relative;
                div {
                    height: 60px;
                    width: 60px;
                    line-height: 60px;
                    text-align: center;
                    background-color: #eaeefb;
                    color: #2f55d4;
                    border-radius: 10px;
                    font-size: 22px;
                }
                p {
                    color: #a7afb8;
                }
            }
            .going-up {
                transition: transform 1s;
            }
            .going-up:hover {
                transform: translate(0px, -20px);
                box-shadow: 0 5px 5px -3px #2f55d4;
            }
            &__card > * {
                margin-bottom: 20px;
            }
        }
    }
</style>