<template>
  <table class="table-bordered w-100">
      <thead>
          <th>Save up to 40% by paying weekly</th>
          <th>Standard</th>
          <th>Professional</th>
          <th>Advanced</th>
      </thead>
        <tbody>
            <tr v-for="option in options" :key="option.name">
                <td v-text="option.description"></td>
                <td v-html="getCellValue(option.standard)" :class="{available : isAvailable(option.standard)}"></td>
                <td v-html="getCellValue(option.professional)" :class="{available : isAvailable(option.professional)}"></td>
                <td v-html="getCellValue(option.advanced)" :class="{available : isAvailable(option.advanced)}"></td>
            </tr>
      </tbody>
      <t-foot>
          <td></td>
          <td></td>
          <td></td>
      </t-foot>
  </table>
</template>

<script>
export default {
    name:"table",
    props: ["options"],
    methods: {
      getCellValue(value) {
          if (value === false) {
              return "&#88;";
          } else if (value === true) {
              return "&#10003;";
          } else {
              return value;
          }
      },
      isAvailable(value) {
          if (value === true) {
              return true;
          } else {
              return false;
          }
      }

    }

}
</script>

<style scoped lang="scss">

@import "../../assets/sass/_vars.scss";

    td {
        padding:15px;
        text-align: center;

        &.available {
            color:$main-color;
        }
    }

</style>