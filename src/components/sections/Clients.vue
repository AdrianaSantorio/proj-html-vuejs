<template>
  <section id="collaborations" class="container">
      <div class="row">
          <div class="col-3" v-for="(client,index) in clients" :key="index">
              <a :href="client.url">
                  <img :src="getImageUrl(client.imageUrl)" :alt="client.name" class="img-fluid">
              </a>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name:"Clients",
    props:["clients"],
    methods: {
        getImageUrl(imageUrl) {
            return require(`../../assets/img/${imageUrl}`);
        
        }
    }
}
</script>

<style>

</style>