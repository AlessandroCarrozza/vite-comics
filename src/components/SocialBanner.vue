<script>
export default {
    name: "SocialBanner",
    data() {
        return {
            socials: ["facebook", "periscope", "pinterest", "twitter", "youtube"]
        }
    }
}
</script>


<template>
    <div class="social-banner">
        <div class="container">
            <a href="#" class="btn">SIGN-UP NOW!</a>

            <div class="socials">
                <h2>FOLLOW US</h2>

                <ul>
                    <li v-for="social in socials">
                        <a href="#">
                            <img :src="'./src/assets/footer-' + social + '.png'" :alt="social">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins";

.social-banner {
    height: 120px;
    background-color: $bg-social-banner;

    .container {
        @include mixins.flex-ali-center;
        justify-content: space-between;

        .btn {
            background-color: #303030;
            border: 3px solid $color-primary;
            padding: 1.2rem 1.6rem;
            color: $color-secondary;
            font-size: 1.2rem;
        }

        .socials {
            @include mixins.flex-ali-center;

            h2 {
                color: $color-primary;
                padding: 0 1rem;
            }

            ul {
                display: flex;

                li {
                    padding: 0 0.5rem;
                    position: relative;
                    top: 2px;
                }
            }
        }
    }
}
</style>