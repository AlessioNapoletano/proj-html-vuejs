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
        <div class="consulants-service">
            <div class="title d-flex align-center">
                <h1>
                    OUR CONSULANTS CAN HELP YOU
                </h1>

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
    height: 50rem;
    background-color: white;
    position: relative;

    .consulants-service {
        padding-top: 7rem;
        color: $main-blue-color;
        width: 85%;
        height: 100%;

        .title {
            margin-bottom: 7rem;

            h1 {
                font-weight: 800;
            }

            .line {
                margin-left: 2rem;
                width: 1200px;
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
            margin-left: 2rem;

            h2 {
                padding: 1rem 0;
                font-weight: 800;
            }

        }

        /*
        <div class="image">
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

        */


    }
}
</style>