<script>
//import ServiceComponent from './ServiceComponent.vue'

export default {
    /*component: {
        ServiceComponent
    },*/

    data() {
        return {
            serviceList:
                [
                    {
                        // Statistical icon: <i class="fa-brands fa-think-peaks"></i>
                        image: 'fa-brands fa-think-peaks',
                        title: 'STATISTICAL CONSULTING',
                        description: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                    },
                    {
                        //Megaphone icon: <i class="fa-solid fa-bullhorn"></i>
                        image: 'fa-solid fa-bullhorn',
                        title: 'DIGITAL CONSULTING',
                        description: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                    },
                    {
                        //Wallet icon: <i class="fa-regular fa-wallet"></i>
                        image: 'fa-solid fa-wallet',
                        title: 'BANKING CONSULTING',
                        description: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                    },
                    {
                        //Enterprise icon: <i class="fa-solid fa-arrows-to-dot"></i>
                        image: 'fa-solid fa-arrows-to-dot',
                        title: 'ENTERPRISE CONSULTING',
                        description: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                    }
                ]
        }
    }

}
</script>

<template>
    <section class="advisory-service d-flex justify-end">
        <div class="container-sm consulants-service">
            <div class="title d-flex align-center">
                <div class="text">
                    <h1>
                        OUR CONSULANTS CAN HELP YOU
                    </h1>
                </div>

                <div class="line"></div>
            </div>

            <div class="box-service d-flex flex-wrap">
                <article v-for="service in serviceList" class="service d-flex">
                    <div class="image d-flex justify-center align-center">
                        <i :class="service.image"></i>
                    </div>

                    <div class="body">
                        <h2>
                            {{ service.title }}
                        </h2>

                        <p>
                            {{ service.description }}
                        </p>
                    </div>

                </article>
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section {
    position: relative;

    .consulants-service {
        padding: 7rem 0rem 3rem 10rem;
        background-color: $main-white-color;

        .title {
            margin-bottom: 7rem;

            .text {
                width: 26%;

                h1 {
                    font-weight: 800;
                }
            }

            .line {
                margin-left: 1rem;
                width: 74%;
                border: 2px solid $line-light-blue;
            }
        }
    }

    .service {
        width: calc(100% / 2);
        height: 18rem;

        .image {
            width: 72px;
            height: 64px;
            border-radius: 100%;

            background-color: $main-red-color;

            i {
                font-size: 2rem;
                color: $main-white-color;
            }
        }

        .body {
            width: 43%;
            margin-left: 3rem;

            h2 {
                padding-bottom: 1rem;
                font-weight: 800;
                color: $main-blue-color;
            }

            p {
                color: $secondary-grey-color;
            }
        }
    }
}
</style>