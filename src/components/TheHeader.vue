<script>
export default {
    name: "TheHeader",
    data() {
        return {
            navLinks: [
                {
                    href: "#characters",
                    text: "characters",
                },
                {
                    href: "#comics",
                    text: "comics",
                },
                {
                    href: "#movies",
                    text: "movies",
                },
                {
                    href: "#tv",
                    text: "tv",
                },
                {
                    href: "#games",
                    text: "games",
                },
                {
                    href: "#collectibles",
                    text: "collectibles",
                },
                {
                    href: "#videos",
                    text: "videos",
                },
                {
                    href: "#fans",
                    text: "fans",
                },
                {
                    href: "#news",
                    text: "news",
                },
                {
                    href: "#shop",
                    text: "shop",
                },
            ]
        }
    }
}
</script>


<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="Logo Comics">
            </div>

            <ul class="navbar">
                <li v-for="link in navLinks">
                    <a class="nav-link" :href="link.href">{{ link.text }}</a>
                    <div class="line"></div>
                </li>
            </ul>
        </div>
    </header>
</template>


<style scoped lang="scss">
header {
    height: 120px;
    background-color: white;

    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;

        img {
            height: 80px;
        }

        .navbar {
            display: flex;
            height: 100%;
        }

        li {
            height: 100%;
            margin: 0 1rem;
            position: relative;
            text-transform: uppercase;

            a {
                color: black;
                text-decoration: none;
                height: 100%;
                display: block;
                display: flex;
                align-items: center;
                font-size: 0.8rem;
                font-weight: 600;

                &:hover {
                    color: #0c7cec;
                }
            }

            .line {
                position: absolute;
                width: 100%;
                height: 7px;
                background-color: #0c7cec;
                bottom: 0;
                display: none;
            }

            &:hover .line {
                display: block;
            }
        }
    }

}
</style>