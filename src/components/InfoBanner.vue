<script>
export default {
    name: "InfoBanner",
    data() {
        return {
            infos: [
                {
                    src: "buy-comics-digital-comics.png",
                    text: "digital comics",
                },
                {
                    src: "buy-comics-merchandise.png",
                    text: "dc merchandise",
                },
                {
                    src: "buy-comics-subscriptions.png",
                    text: "subscription",
                },
                {
                    src: "buy-comics-shop-locator.png",
                    text: "shop locator",
                },
                {
                    src: "buy-dc-power-visa.svg",
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
                <img :src="'./src/assets/' + info.src">
                <span>{{ info.text }}</span>
            </li>
        </ul>
    </div>
</template>


<style scoped lang="scss">
.info-banner {
    height: 180px;
    background-color: #0282f9;

    .container {
        display: flex;
        align-items: center;
        justify-content: space-around;

        li {
            display: flex;
            align-items: center;
            color: white;
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