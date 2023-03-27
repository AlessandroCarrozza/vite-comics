<script>
export default {
    name: "TheFooter",
    data() {
        return {
            dcComicsLinks: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
            shopLinks: ["Shop DC", "Shop DC Collectibles"],
            dcLinks: ["Terms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs",
                "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
            sitesLinks: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]
        }
    }
}
</script>


<template>
    <footer>
        <div class="container">
            <!-- <img src="../assets/dc-logo.png" alt="Logo Comics rotate"> -->

            <div class="links">
                <div class="side-links">
                    <ul>
                        <h1>DC COMICS</h1>
                        <li v-for="link in dcComicsLinks"><a href="#">{{ link }}</a></li>
                    </ul>
                    <ul>
                        <h1>SHOP</h1>
                        <li v-for="link in shopLinks"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>

                <div class="side-links">
                    <ul>
                        <h1>DC</h1>
                        <li v-for="link in dcLinks"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>

                <div class="side-links">
                    <ul>
                        <h1>SITES</h1>
                        <li v-for="link in sitesLinks"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>


<style scoped lang="scss">
footer {
    background-image: url("../assets/footer-bg.jpg");
    background-size: cover;

    .container {
        position: relative;
        padding: 4rem 0;

        // img {
        //     transform: rotate(-30deg);
        //     opacity: 0.5;
        //     height: 500px;
        //     position: absolute;
        //     right: 0;
        //     top: -50px;
        //     bottom: -50px;
        //     z-index: 0;
        // }

        .links {
            display: flex;

            .side-links {
                padding-right: 5rem;
            }

            h1 {
                color: white;
                padding: 1rem 0;
            }

            li {
                padding: 3px 0;
            }

            a {
                color: #c4ccd1;
                font-size: 0.9rem;

                &:hover {
                    text-decoration: underline;
                }
            }
        }

    }

}
</style>