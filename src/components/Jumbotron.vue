<script>
export default {
    name: "Jumbotron",
}
</script>



<template>
    <div class="jumbotron"></div>
</template>



<style scoped lang="scss">
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins";

.jumbotron {
    height: 400px;
    background-image: url("../assets/jumbotron.jpg");
    background-size: cover;
}
</style>