<script>
export default {

}
</script>

<template>
    <section class="deliver-care">
        <div class="wrapper d-flex align-center justify-between">
            <div class="slogan">
                <h1>
                    WE HELP TO DELIVER THE BUSINESS CASE
                </h1>
            </div>
            <div class="description">
                <p>
                    When, while lovely valley teems with vapour around meand meridian sun strikes the upper impenetrable
                    foliage of my trees, and but a thousand unkown
                </p>
            </div>

        </div>

        <div class="button">
            <button class="btn">
                GET STARTED
            </button>
        </div>

    </section>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section.deliver-care {
    background-color: $line-light-blue;
    padding: 8rem 0;
    width: 90%;
    margin-bottom: 13rem;

    position: relative;

    .wrapper {
        width: 60%;
        margin: 0 auto;
    }

    .slogan {
        width: 45%;


        h1 {
            font-size: 2.5rem;
        }
    }

    .description {
        width: 40%;
        font-size: 1.1rem;
    }

    .button {
        position: absolute;
        bottom: 0px;
        right: 0px;

        &:hover .btn {
            background-color: $main-blue-color;
        }

        .btn {
            border: none;
            background-color: $main-red-color;
            color: $main-white-color;
            cursor: pointer;
            transition: .5s;
            padding: 1.5rem 4rem;
            font-size: 1.1rem;
            border: none;
        }
    }
}
</style>