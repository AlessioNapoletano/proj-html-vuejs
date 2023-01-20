<script>
export default {
    name: 'MainProject',
    data() {
        return {
            imageList: ['DRY-1-790x592.jpg', '221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg', 'z1el4c4p-790x592.jpg']
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
    <section class="project container">
        <div class="small-text d-flex">
            <div class="line"></div>
            <p>
                PROJETC
            </p>
        </div>

        <div class="big-text d-flex justify-between">
            <div class="text">
                <h1>
                    OUR EXPER TRUSTED CONSULATNTS HELP CLIENTS
                </h1>
            </div>

            <div class="icon d-flex justify-end align-start">
                <button>
                    <i class="fa-solid fa-arrow-left"></i>
                </button>

                <button>
                    <i class="fa-solid fa-arrow-right"></i>
                </button>
            </div>

        </div>

        <div class="image-wrapper d-flex">
            <div class="image" v-for="image in imageList">
                <img :src="getImagePath(image)" alt="project logo image">
            </div>
        </div>
    </section>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section {
    margin-bottom: 15rem;
    color: $main-white-color;

    .small-text {
        font-size: 1.2rem;
        display: flex;
        align-items: center;
        margin-bottom: 2rem;

        .line {
            margin: .9rem 1rem 0 0;
            width: 50px;
            border: 2px solid $line-light-blue;
        }
    }

    .big-text {
        margin-bottom: 3rem;

        .text {
            width: 50%;

            h1 {
                font-size: 2.5rem;
            }

        }

        .icon {
            button {
                border: none;
                background-color: $secondary-grey-color;
                color: white;
                padding: 1rem;
                cursor: pointer;
            }

            button:first-child {
                margin-right: .5rem;
            }

        }
    }

    .image-wrapper {
        justify-content: space-around;

        .image {
            width: calc((100% / 3));
            height: 22rem;

            &:nth-child(2) {
                margin: 0 1.5rem;
            }

            img {
                width: 100%;
                height: auto;
            }
        }
    }
}
</style>