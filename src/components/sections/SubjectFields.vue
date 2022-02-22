<template>
  <section id="subject-fields" class="container">
          <div class="row">
            <div v-for="card in cards" :key="card.id" class="col-2">
                <Card :item="card" />
            </div>
      </div>
      </section>
</template>

<script>
import Card from "./Card.vue"

export default {
    name:"Subject Fields",
    props: ["cards"],
    components: {
        Card,
    }
}
</script>

<style>

</style>