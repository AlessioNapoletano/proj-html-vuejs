<script>
export default {

}
</script>

<template>

    <section class="about-us d-flex">
        <div class="left-box"></div>

        <div class="right-box d-flex align-center justify-center">
            <div class="slogan">
                <div class="small-text d-flex">
                    <div class="line"></div>
                    <h3>
                        ABOUT US
                    </h3>
                </div>

                <div class="big-text">
                    <h1>
                        WE MAKE YOUR STRATEGY WORK
                    </h1>
                </div>

                <div class="description">
                    <p>
                        When, while lovely valley teems with vapour around meand eridian sun strikes the upper
                        impenetrable foliage of my trees, and but a thousand unknow plants are noticed when i hear the
                        buzz of the little world among the stalks, and grow familiar indescribable forms of the insects
                        and flies, then i feel the presence of the almighty .
                    </p>
                </div>
            </div>
        </div>

    </section>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section {
    height: 55rem;
    color: $main-white-color;

    .left-box {
        width: 58%;
        height: 100%;

        background-image: url('../assets/images/business-people-working-together-on-project-and-5FHSKBL.jpg');
        background-repeat: no-repeat;
    }

    .right-box {
        width: 42%;
        height: 100%;
        padding-left: 3rem;
        padding-right: 3rem;

        .slogan {
            width: 80%;
            height: 50%;
        }
    }

    .small-text {
        margin-bottom: 1rem;

        .line {
            margin: .9rem 1rem 0 0;
            height: 0;
            width: 50px;
            border: 2px solid $line-light-blue;
        }
    }

    .big-text {
        font-size: 2.8rem;
        margin-bottom: 2rem;
    }

    .description {
        color: $main-grey-color;
        font-size: 1.3rem;
    }


}
</style>