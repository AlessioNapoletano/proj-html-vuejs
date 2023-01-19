<script>
export default {
    name: 'MainBlog',
    data() {
        return {
            blogList:
                [
                    {
                        image: 'startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg',
                        date: 'july 4, 2019',
                        creator: 'by paul',
                        title: 'Canadian Consulting Firm acquired by Uk Giant',
                        description: 'When, While lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...'
                    },

                    {
                        image: 'business-people-working-together-on-project-and-5FHSKBL-1390.jpg',
                        date: 'july 4, 2019',
                        creator: 'by paul',
                        title: 'Canadian Consulting Firm acquired by Uk Giant',
                        description: 'When, While lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...'
                    }
                ]
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
    <section class="blog">
        <div class="container">
            <div class="small-text d-flex align-end">
                <div class="line"></div>
                <p>
                    BLOG
                </p>
            </div>

            <div class="wrapper d-flex justify-between align-center">
                <div class="big-text">
                    <h1>
                        THE RECENT NEWS YOU MUST READ IT
                    </h1>
                </div>

                <div class="button">
                    <button>
                        VIEW ALL
                    </button>
                </div>
            </div>

            <div class="image-wrapper justify-between d-flex flex-wrap">
                <div class="image" v-for="blogArticle in blogList">
                    <img :src="getImagePath(blogArticle.image)" alt="Image's article">

                    <div class="box-description">
                        <p class="heading d-inline">
                            {{ blogArticle.date }}
                        </p>

                        <p class="heading d-inline ">
                            {{ blogArticle.creator }}
                        </p>

                        <h2>
                            {{ blogArticle.title }}
                        </h2>

                        <p class="description">
                            {{ blogArticle.description }}
                        </p>
                    </div>
                </div>



            </div>

        </div>


    </section>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section.blog {
    margin-top: 10rem;
    height: 50rem;
    color: $main-white-color;

    .container {
        height: 100%;

        .small-text {
            font-size: 1.2rem;
            margin-bottom: 2rem;

            .line {
                margin: .9rem 1rem 0 0;
                width: 50px;
                height: 0;
                border: 2px solid $line-light-blue;
            }
        }

        .wrapper {
            margin-bottom: 3rem;

            .big-text {
                margin-bottom: 1rem;

                h1 {
                    font-size: 3rem;
                }
            }


            button {
                background-color: $line-light-blue;
                padding: 1.6rem 4.5rem;
                border: none;
                font-size: 1.05rem;
            }
        }


        .image-wrapper {

            .image {
                position: relative;
                width: 49%;
                height: 100%;

                img {
                    width: 100%;
                    height: auto;
                }

                .box-description {
                    position: absolute;
                    top: 65%;
                    right: 0;
                    width: 591px;
                    height: 299px;

                    padding: 4rem 10rem 0 6rem;

                    background-color: $main-white-color;

                    .heading {
                        color: $main-red-color;
                        margin: 0 2rem 0 0;
                        font-weight: bold;
                    }

                    h2 {
                        color: $main-black-color;
                        margin: 1.4rem 0 1.8rem 0;
                    }

                    .description {
                        color: $main-grey-color;
                    }

                }
            }


        }

    }

}
</style>