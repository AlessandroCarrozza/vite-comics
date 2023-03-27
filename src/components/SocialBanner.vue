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
.social-banner {
    height: 120px;
    background-color: #303030;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .btn {
            background-color: #303030;
            border: 3px solid #0282f9;
            padding: 1.2rem 1.6rem;
            color: white;
            font-size: 1.2rem;
        }

        .socials {
            display: flex;
            align-items: center;

            h2 {
                color: #0282f9;
                padding: 0 1rem;
            }

            ul {
                display: flex;

                li {
                    padding: 0 0.5rem;
                }
            }
        }
    }
}
</style>