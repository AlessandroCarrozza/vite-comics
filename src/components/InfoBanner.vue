<script>
export default {
    name: "InfoBanner",
    data() {
        return {
            infos: [
                {
                    src: "comics-digital-comics.png",
                    text: "digital comics",
                },
                {
                    src: "comics-merchandise.png",
                    text: "dc merchandise",
                },
                {
                    src: "comics-subscriptions.png",
                    text: "subscription",
                },
                {
                    src: "comics-shop-locator.png",
                    text: "shop locator",
                },
                {
                    src: "dc-power-visa.svg",
                    text: "dc power visa",
                },
            ]
        }
    }
}
</script>


<template>
    <div class="info-banner">
        <ul class="container">
            <li v-for="info in infos">
                <img :src="'./src/assets/buy-' + info.src" :alt="info.text">
                <span>{{ info.text }}</span>
            </li>
        </ul>
    </div>
</template>


<style scoped lang="scss">
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins";

.info-banner {
    height: 180px;
    background-color: $color-primary;

    .container {
        @include mixins.flex-ali-center;
        justify-content: space-around;

        li {
            display: flex;
            align-items: center;
            color: $color-secondary;
            text-transform: uppercase;
            font-size: 0.9rem;

            img {
                height: 60px;
                padding: 0 0.5rem;
            }
        }
    }
}
</style>