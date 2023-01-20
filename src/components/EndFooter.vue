<script>
export default {
    name: 'EndFooter',
    data() {
        return {
            navList: ['Terms of use', 'Privacy Environmental Policy']
        }
    },
}
</script>

<template>
    <section class="end-footer">
        <div class="container">
            <hr>
            <div class="wrapper d-flex justify-between ">
                <nav>
                    <ul>
                        <li v-for="item in navList">
                            <a href="#"> {{ item }}</a>
                        </li>
                    </ul>
                </nav>

                <div class="copyright">
                    <p>
                        CopyRight &copy; 2023 Phlox Consulting. All Rights Reserved.
                    </p>
                </div>

            </div>


        </div>

    </section>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section.end-footer {
    color: $main-grey-color;
    padding-bottom: 3rem;

    .container {

        hr {
            color: $main-grey-color;
            margin-bottom: 2rem;
        }

        li {
            margin-bottom: .2rem;

            a {
                color: $main-grey-color;
            }


        }
    }
}
</style>