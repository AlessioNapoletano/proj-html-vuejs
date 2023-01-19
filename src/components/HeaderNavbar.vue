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
                <li v-for="item in navList" :class="(item.current) ? 'current-selected' : ''"> {{
                    item.name
                }}
                </li>
            </ul>
        </nav>
    </div>
</template>


<style lang="scss" scoped>
.container {
    position: absolute;
}

img {
    margin-top: .5rem;
    width: 200px;
}

li {
    display: inline;
    list-style-type: none;
    padding: 1rem;
    cursor: pointer;
}

.current-selected {
    font-weight: bold;
    border-top: 2px solid black;
}
</style>