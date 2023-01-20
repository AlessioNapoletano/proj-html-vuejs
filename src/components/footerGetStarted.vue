
<script>
export default {
    name: 'FooterGetStarted',
}
</script>

<template>
    <section class="get-started">
        <div class="wrapper d-flex justify-center flex-column align-center">
            <h1>
                LET'S TALK ABOUT WORK
            </h1>

            <p>
                A wonderful serenity has taken possession Far far away, behind the word mountains.
            </p>

            <button>
                GET STARTED
            </button>
        </div>

    </section>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section {
    background-image: url('../assets/images/business-people-working-together-on-project-and-B3MZ4TX.jpg');
    background-repeat: no-repeat;
    height: 30rem;
    color: $main-white-color;
    margin-bottom: 6rem;

    .wrapper {
        width: 30%;
        margin: 0 auto;
        padding-top: 10rem;


        h1 {
            font-size: 2.6rem;
            margin-bottom: 1rem;
        }

        p {
            margin-bottom: 1rem;
            font-size: 1.2rem;
            text-align: center;
            padding: 0 5rem;

        }

        button {
            border: none;
            font-size: 1.1rem;
            padding: 1.5rem 3.3rem;
            background-color: $main-blue-color;
            color: $main-white-color;
        }
    }


}
</style>