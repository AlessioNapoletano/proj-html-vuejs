<script>
export default {
    data() {
        return {
            navList:
                [
                    {
                        name: 'HOME',
                        current: true,
                    },

                    {
                        name: 'ABOUT',
                        current: false,
                    },

                    {
                        name: 'PROJECTS',
                        current: false,
                    },

                    {
                        name: 'SERVICES',
                        current: false,
                    },

                    {
                        name: 'BLOG',
                        current: false,
                    },

                    {
                        name: 'CONTACT',
                        current: false,
                    },
                ]
        }
    },
}
</script>

<template>
    <div class="container justify-between d-flex">
        <div class="logo">
            <img src="../assets/images/logotype.png" alt="Logo">
        </div>

        <nav>
            <ul class="d-flex">
                <li v-for="item, index in navList" :key="index" :class="(item.current) ? 'current-selected' : ''"
                    @mouseover="item.current = true" @mouseleave="item.current = false">
                    <a href="#">
                        {{ item.name }}
                    </a>
                </li>
            </ul>
        </nav>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.container {
    position: absolute;
    color: $main-white-color;
    z-index: 1;
    left: 10%;

    .logo {
        padding-top: 1.5rem;

        img {
            width: 150px;
        }
    }
}

li {
    padding-top: 1.5rem;
    margin: 0 1rem 1rem 1rem;
    cursor: pointer;

    &:hover li {
        border-top: 3px solid $main-white-color;
        font-weight: bold;
    }

    a {
        color: $main-white-color;
    }
}

.current-selected {
    font-weight: bold;
    border-top: 3px solid $main-white-color;
}
</style>