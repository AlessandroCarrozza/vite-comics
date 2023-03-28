<script>
export default {
    name: "SingleCard",
    props: {
        image: String,
        title: String
    }
}
</script>



<template>
    <img :src="image" alt="Comics Photo">
    <h5>{{ title }}</h5>
</template>



<style scoped lang="scss">
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins";

img {
    width: 100%;
    height: 170px;
}

h5 {
    color: $color-secondary;
    text-transform: uppercase;
}
</style>