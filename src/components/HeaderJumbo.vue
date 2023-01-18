
<script>
export default {

}
</script>

<template>
    <div class="wrapper d-flex">
        <div class="left-box">
            <div class="slogan">
                <div class="small-text d-flex">
                    <div class="line"></div>
                    <p>
                        ALWATS THE BEST WAY YOU NEED IT
                    </p>
                </div>

                <div class="big-text">
                    <h1>
                        THE BEST BUSINESS CONSULTING
                    </h1>
                </div>

                <div class="button-icon d-flex">
                    <button class="btn">
                        READ MORE
                    </button>

                    <div class="icon">
                        <i class="fa-solid fa-play"></i>
                    </div>
                </div>


            </div>

        </div>

        <div class="right-box">

        </div>

    </div>


</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.left-box {
    width: 30%;
    height: 60rem;
    background-color: $main-blue-color;
    color: $main-white-color;
    position: relative;

    .slogan {
        position: relative;
        top: 306px;
        left: 124px;

        .small-text {
            font-size: 1.2rem;
            display: flex;
            align-items: center;

            .line {
                margin: .9rem 1rem 0 0;
                width: 50px;
                border: 2px solid $line-light-blue;
            }
        }

        .big-text {
            margin-bottom: 1rem;

            h1 {
                font-size: 6rem;
            }
        }

        .button-icon {
            .btn {
                padding: 1.5rem 4rem;
                font-size: 1.1rem;
                background-color: $line-light-blue;
                border: none;
                margin-right: 2rem;
            }

            .icon {
                font-size: 1rem;
                border: 2px solid $main-white-color;
                border-radius: 100%;
                padding: .6rem 1.5rem;

                i {
                    color: $line-light-blue;
                    margin-top: .9rem;
                }
            }
        }
    }
}

.right-box {
    width: 70%;
    height: 60rem;
    background-image: url('../assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}
</style>