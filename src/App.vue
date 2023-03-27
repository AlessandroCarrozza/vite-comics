<script>

import TheHeader from "./components/TheHeader.vue"
import TheMain from "./components/TheMain.vue"
import InfoBanner from "./components/InfoBanner.vue"
import TheFooter from "./components/TheFooter.vue"
import SocialBanner from "./components/SocialBanner.vue"

export default {
  components: {
    TheHeader,
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

  <TheMain></TheMain>

  <InfoBanner></InfoBanner>

  <TheFooter></TheFooter>

  <SocialBanner></SocialBanner>
</template>



<style></style>
