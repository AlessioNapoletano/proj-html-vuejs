<script>
export default {
    name: 'MainTestimonial',

    data() {
        return {
            feedbackList:
                [
                    {
                        feed: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when i hear the buzz of the little.',
                        name: 'Vera Duncan',
                        company: 'Amazon Inc.'
                    },
                    {
                        feed: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when i hear the buzz of the little.',
                        name: 'Vera Duncan',
                        company: 'Amazon Inc.'
                    },
                    {
                        feed: 'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when i hear the buzz of the little.',
                        name: 'Vera Duncan',
                        company: 'Amazon Inc.'
                    }
                ]
        }
    },
}
</script>

<template >
    <section class="testimonial d-flex justify-end">
        <div class="container">
            <div class="small-text">
                <div class="small-text d-flex align-center">
                    <p>
                        TESTIMONIAL
                    </p>

                    <div class="line"></div>
                </div>
            </div>

            <div class="wrapper d-flex justify-end">
                <div class="big-text">
                    <h1>
                        WHAT'S THE CUSTOMER SAY ABOUT OUR WORK
                    </h1>
                </div>

            </div>
        </div>
    </section>

    <section class="costumer-feedback">
        <div class="wrapper d-flex">
            <div class="costumer" v-for="feedback in feedbackList">
                <p>
                    {{ feedback.feed }}
                </p>

                <h2>
                    {{ feedback.name }}
                </h2>

                <p>
                    {{ feedback.company }}
                </p>
            </div>
        </div>


    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section.testimonial {
    color: $main-white-color;
    margin-bottom: 2rem;

    .container {

        .small-text {
            margin-bottom: 2rem;

            p {
                margin: 0 auto;
                font-size: 1.2rem;
            }

            .line {
                height: 0;
                width: 50px;
                border: 2px solid $line-light-blue;

            }
        }

        .big-text {
            width: 45%;
            text-align: end;

            h1 {
                font-size: 3rem;
            }
        }
    }
}

section.costumer-feedback {
    background-color: $main-white-color;
    width: 90%;
    margin-inline-start: auto;
    margin-bottom: 14rem;

    .wrapper {
        width: 90%;

        .costumer {
            width: calc(100%/3);
            padding: 3rem 5rem;
            font-size: 1.1rem;

            p {
                margin-bottom: 2.5rem;
            }

            h2 {
                margin-bottom: .5rem;
                font-weight: 800;
            }
        }
    }

}
</style>