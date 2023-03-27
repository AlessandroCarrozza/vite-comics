<script>
export default {
    name: "TheMain"
}
</script>


<template>
    <main>
        <div class="container">
            <h1>Content goes here</h1>
        </div>
    </main>
</template>


<style scoped lang="scss">
main {
    height: 150px;
    background-color: #1c1c1c;

    .container {
        display: flex;
        align-items: center;

        h1 {
            color: white;
        }
    }

}
</style>