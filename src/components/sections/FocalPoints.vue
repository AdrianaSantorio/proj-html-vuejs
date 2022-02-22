<template>
  <section class="focal-points">
          <div class="container">
              <div class="row">
                  <div class="col-3">
                      <!-- Navbar -->
                      <VerticalNavbar :links="focalPoints" />
                  </div>
                  <div class="col-9">
                      <!-- section title -->
                       <h2>Learning Possibilities</h2>
                       <!-- section text -->
                       <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Beatae non voluptates, unde cumque reiciendis necessitatibus. Reprehenderit maiores iure sapiente sit omnis! Porro veniam facilis praesentium. Doloremque, fugiat illum? Magnam, id?</p>

                       <div class="d-flex justify-content-between align-items-end ">
                            <ul class="">
                                <li>We enrich lives through learning.</li>
                                <li>Maximizing potential through individual attention.</li>
                                <li>The trusted name for specialized training.</li>
                                <li>People teach. People learn. This is were they connect.</li>
                            </ul>
                            <img src="../../assets/img/h12-tabs-icon-1.png" class="img-fluid">
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

.col-3 {
    padding-right: 40px;
}

.focal-points {

    color: $t-color-gray;

    p {
        margin: 30px 0;
    }

    img {
        width: 120px;
    }

    ul{
        padding: 0;

        li{
            margin-bottom: 20px;
            font-size: 1.1rem;
            

            &::before {
                content: '\2713';
                color: $main-color;
                margin-right: 4px;
            }
        }
    }
}


</style>