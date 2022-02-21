<template>
  <nav>
        <!-- barra di navigazione -->
        <ul class="w-100">
            <li v-for="(menu, index) in menus" :key="index">
                <a href="#">{{menu.toUpperCase()}}</a>
            </li>
        </ul>
  </nav>
</template>

<script>
export default {
    name:"Navbar",
    props: ["menus"],



}
</script>

<style scoped lang="scss">

@import "../assets/sass/_mixins.scss";


ul {
    @include flex-between;
    margin: 0;
    li {
        font-weight: 400;
        font-size: 1.2rem;
    }
    
}

</style>