<template>
  <div class="cards">
      <img :src="getImageUrl(item.imageUrl)" alt="field" class="img-fluid">
      <h6>{{item.name}}</h6>
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
    .cards {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: #F2F8FC;
    }
</style>