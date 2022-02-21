<template>
  <section class="focal-points">
          <div class="container">
              <div class="row">
                  <div class="col-3 h-100">
                      <!-- Navbar -->
                      <VerticalNavbar :links="focalPoints" />
                  </div>
                  <div class="col-9">
                      <!-- section title -->
                       <h2>Learning Possibilities</h2>
                       <!-- section text -->
                       <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Beatae non voluptates, unde cumque reiciendis necessitatibus. Reprehenderit maiores iure sapiente sit omnis! Porro veniam facilis praesentium. Doloremque, fugiat illum? Magnam, id?</p>

                       <div>
                            <ul>
                                <li>We enrich lives through learning.</li>
                                <li>Maximizing potential through individual attention.</li>
                                <li>The trusted name for specialized training.</li>
                                <li>People teach. People learn. This is were they connect.</li>
                            </ul>
                            <img src="../../assets/img/h12-tabs-icon-1.png" alt="">
                       </div>
                  </div>
              </div>
          </div>
  </section>
</template>

<script>

import VerticalNavbar from "./VerticalNavbar.vue"

export default {
    name: "FocalPoints",
    components: {
        VerticalNavbar,
    },
    props: ["focalPoints"],

}
</script>

<style scoped lang="scss">

@import "../../assets/sass/_vars.scss";

.focal-points {
    ul{
        li{
            &::before {
                content: '\2713';
                color: $main-color;
                margin-right: 4px;
            }
        }
    }
}

</style>