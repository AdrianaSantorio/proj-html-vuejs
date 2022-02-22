<template>
  <footer>
      <UpperFooter />
      <BottomFooter />
  </footer>
</template>

<script>

import BottomFooter from "./footer/BottomFooter.vue"
import UpperFooter from "./footer/UpperFooter.vue"

export default {
    name:"Footer",
    components: {
        BottomFooter,UpperFooter,
    }
}
</script>

<style scoped lang="scss">
    @import "../assets/sass/_vars.scss";

    footer {
        background-color: $bg-color-d-gray;
        color: white;
    }
</style>