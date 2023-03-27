<script>
export default {
    name: "TheHeader",
    data() {
        return {
            navLinks: [
                {
                    href: "#characters",
                    text: "CHARACTERS",
                },
                {
                    href: "#comics",
                    text: "COMICS",
                },
                {
                    href: "#movies",
                    text: "MOVIES",
                },
                {
                    href: "#tv",
                    text: "TV",
                },
                {
                    href: "#games",
                    text: "GAMES",
                },
                {
                    href: "#collectibles",
                    text: "COLLECTIBLES",
                },
                {
                    href: "#videos",
                    text: "VIDEOS",
                },
                {
                    href: "#fans",
                    text: "FANS",
                },
                {
                    href: "#news",
                    text: "NEWS",
                },
                {
                    href: "#shop",
                    text: "SHOP",
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
        max-width: 1170px;
        margin: auto;
        height: 100%;
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
            list-style: none;
            height: 100%;
            margin: 0 1rem;
            position: relative;

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