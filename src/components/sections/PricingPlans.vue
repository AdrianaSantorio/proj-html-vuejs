<template>
  <section id="pricing-plans" class="container text-center">
      <!-- section title -->
      <h2>Pricing Plans</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquid voluptatibus quos quidem commodi.</p>
      <Table :options="options"/>
  </section>
</template>

<script>
import Table from "./Table.vue"

export default {
    name:"Pricing Plans",
    props: ["options"],
    components: {
        Table,
    }
}
</script>

<style>

</style>