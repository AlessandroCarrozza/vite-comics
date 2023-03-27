<script>
export default {
    name: "TheHeader"
}
</script>


<template>
    <header>
        <div class="container">
            <div class="logo">Logo</div>

            <ul class="navbar">
                <li><a class="nav-link" href="#">Testo</a></li>
                <li><a class="nav-link" href="#">Testo</a></li>
                <li><a class="nav-link" href="#">Testo</a></li>
                <li><a class="nav-link" href="#">Testo</a></li>
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
    }

    .navbar {
        display: flex;
        height: 100%;
    }

    li {
        list-style: none;
        height: 100%;
        margin: 0 1rem;

        a {
            color: black;
            text-decoration: none;
            height: 100%;
            display: block;
            display: flex;
            align-items: center;
        }
    }
}
</style>