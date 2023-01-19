<script>
export default {

}
</script>

<template>
    <section class="deliver-care d-flex align-center justify-around">
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
        <div class="button">
            <button>
                GET STARTED
            </button>
        </div>

    </section>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section.deliver-care {
    background-color: $line-light-blue;
    height: 20rem;
    width: 90%;

    position: relative;

    .slogan {
        width: 25%;

        h1 {
            font-size: 2.5rem;
        }
    }

    .description {
        width: 23%;
    }

    .button {
        position: absolute;
        bottom: 0px;
        right: 0px;

        button {
            border: none;
            background-color: $main-red-color;
            color: $main-white-color;
            padding: 1rem 2rem;
            cursor: pointer;
        }
    }
}
</style>