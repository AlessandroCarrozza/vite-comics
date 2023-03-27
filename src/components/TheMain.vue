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
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins";

main {
    height: 150px;
    background-color: #1c1c1c;

    .container {
        @include mixins.flex-ali-center;

        h1 {
            color: $color-secondary;
        }
    }

}
</style>