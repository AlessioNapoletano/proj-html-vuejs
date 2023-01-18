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
                        image: '',
                        title: 'STATISTICAL CONSULTING',
                        description: 'when, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                    },
                    {
                        image: '',
                        title: 'DIGITAL CONSULTING',
                        description: 'when, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                    },
                    {
                        image: '',
                        title: 'BANKING CONSULTING',
                        description: 'when, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
                    },
                    {
                        image: '',
                        title: 'ENTERPRISE CONSULTING',
                        description: 'when, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a'
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
                <article class="service">
                    <div class="image">
                        <!--immagine-->
                    </div>

                    <div class="body">
                        <h2>
                            <!--title-->
                        </h2>

                        <p>
                            <!--body-->
                        </p>
                    </div>

                </article>

                <article class="service">

                </article>

                <article class="service">

                </article>

                <article class="service">

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
        border: 1px solid black;
        height: 100%;

        .line {
            margin-left: 2rem;
            width: 1206px;
            border: 2px solid $line-light-blue;
        }

        .box-service {
            .service {
                width: calc(100% / 2);
                border: 1px solid black;
                height: 18rem;
            }
        }
    }
}
</style>