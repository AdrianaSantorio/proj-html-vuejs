<template>
  <div class="cards">
      <a href="#"><img :src="getImageUrl(item.imageUrl)" alt="field" class="img-fluid"></a>
      <a href="#"><h6>{{item.name}}</h6></a>
  </div>
</template>

<script>
export default {
    name:"Card",
    props: ["item"],
    methods: {
        getImageUrl(imageUrl) {
            return require(`../../assets/img/${imageUrl}`);
        
        }
    }
    
}
</script>

<style scoped lang="scss">
    @import "../../assets/sass/_vars.scss";

    .cards {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: $bg-color-gray-cards;
        padding: 50px;
         h6 {
             font-size: 1.1rem;
             margin-top: 1.6rem;
         }
    }
</style>