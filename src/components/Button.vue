<template>
  <a href="#">
      {{buttonText.toUpperCase()}}
  </a>
</template>

<script>
export default {
    name: "Button",
    props: ["buttonText"]
}
</script>

<style scoped lang="scss">

@import "../assets/sass/_vars.scss";
    a {
        display: inline-block;
        background-color:$main-color;
        color:white;
        min-width: 150px;
        padding: 10px;
        font-weight: 500;
    }
</style>