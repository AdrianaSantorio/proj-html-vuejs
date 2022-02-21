<template>
    <!-- Upper header -->
  <div id="upper-header">
        <!-- logo -->
        <Logo />
        <!-- navbar -->
        <HorizontalNavbar :menus="menus" class="navbar"/>
        <!-- funzioni? -->
  </div>
</template>

<script>
import HorizontalNavbar from "./HorizontalNavbar.vue"
import Logo from "./Logo.vue"

export default {
    name:"UpperHeader",
    components: {
        HorizontalNavbar, Logo,
    },
    props: ["menus"],
}
</script>

<style scoped lang="scss">

@import "../assets/sass/_mixins.scss";

#upper-header {

    @include flex-between;
    height: 150px;

    .navbar {
        flex-grow: 1;
    }

}

</style>