<script>
export default {
    name: 'FooterNav',
    data() {
        return {
            imgPath: 'logotype-2-150x25.png',
            navList: ['HOME', 'ABOUT', 'PROJECTS', 'SERVICES', 'BLOG', 'CONTACT'],
            iconList: ['fa-brands fa-instagram', 'fa-brands fa-linkedin-in', 'fa-brands fa-facebook-f', 'fa-brands fa-twitter']

        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(`../assets/images/${imgPath}`, import.meta.url).href;
        }
    }

}
</script>

<template>
    <section class="footer-nav">
        <div class="container d-flex justify-between">
            <div class="logo">
                <img :src="getImagePath(imgPath)" alt="Logo Icon">
            </div>
            <nav>
                <ul class="d-flex">
                    <li v-for="item in navList">
                        <a href="#">{{ item }}</a>
                    </li>
                </ul>

            </nav>
            <div class="social-icon">
                <a href="#" v-for="icon in iconList">
                    <i :class="icon"></i>
                </a>
            </div>
        </div>

    </section>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section {
    margin-bottom: 6rem;

    .container {

        nav {

            li {
                padding: 0 .8rem;
                font-size: 1.2rem;
            }

            a {
                color: $main-grey-color;
            }

        }

        .social-icon {

            a {
                color: $main-white-color;
                margin-left: .8rem;

                i {
                    font-size: 1.2rem;
                }
            }
        }

    }
}
</style>