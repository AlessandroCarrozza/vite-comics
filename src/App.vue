<script>

import TheHeader from "./components/TheHeader.vue"
import Jumbotron from "./components/Jumbotron.vue"
import TheMain from "./components/TheMain.vue"
import InfoBanner from "./components/InfoBanner.vue"
import TheFooter from "./components/TheFooter.vue"
import SocialBanner from "./components/SocialBanner.vue"

export default {
  components: {
    TheHeader,
    Jumbotron,
    TheMain,
    InfoBanner,
    TheFooter,
    SocialBanner
  },
  data() {

  },
  methods: {

  }
}
</script>



<template>
  <TheHeader></TheHeader>

  <Jumbotron></Jumbotron>

  <TheMain></TheMain>

  <InfoBanner></InfoBanner>

  <TheFooter></TheFooter>

  <SocialBanner></SocialBanner>
</template>



<style lang="scss">
@use "./styles/general.scss"
</style>
