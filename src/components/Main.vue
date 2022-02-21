<template>
  <main>
      <section id="subject-fields" class="container">
          <div class="row">
            <div v-for="card in cards" :key="card.id" class="col-2">
                <Card :item="card" />
            </div>
      </div>
      </section>
      <section id="tutoring" class="container">
          <h3>The Trusted Name 
              <br>
                for In-Home Tutoring</h3>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur distinctio deleniti maiores rem neque dolore sit! Officiis distinctio, perferendis inventore architecto perspiciatis, earum commodi consectetur natus maxime voluptate quam. Minima?</p>
          <a href="#">LEARN MORE</a>
          <figure>
              <img src="../assets/img/h5-img-1.jpg" class="img-fluid w-100" alt="tutoring">
          </figure>
      </section>
      <section id="reviews">
          <div class="container">
              <div class="row">
                <div class="col-6">
                    <!-- section image -->
                    <figure>
                        <img src="../assets/img/h5-img-2.jpg" class="img-fluid" alt="">
                    </figure>
                </div>
                <div class="col-6">
                    <!-- Section title -->
                    <h2>Empowering Children to Reach Their Potential</h2>
                    <!-- Section text -->
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Praesentium, officia cumque adipisci ex eligendi porro doloribus! Facilis ratione sunt, obcaecati commodi excepturi odio, aut id quaerat, sequi iste laborum eveniet?</p>
                    <!-- Counter -->
                    <div id="review-counter">
                        <div class="slider">
                            <div>
                                <div>168</div>
                                <span>User Stories</span>
                            </div>
                            <div>
                                    <div>347</div>
                                    <span>Events</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
          </div>
          <div class="slider">
              <div class="slider-content text-center">
                    <!-- img -->
                    <img src="../assets/img/instructor-img-6.jpg" alt="" class="rounded-circle">
                    <!-- text -->
                    <p>"Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nemo non illo voluptatibus nulla, animi, cupiditate libero perferendis eligendi tempore asperiores cum. Nobis, nesciunt consequatur cumque earum asperiores illum atque ea."</p>
                    <!-- name -->
                    <h6>Joan Collins</h6>
                    <!-- role -->
                    <span>Student</span>
              </div>
          </div>
      </section>
      <FocalPoints :focal-points="focalPoints" />
  </main>
</template>

<script>

import Card from "./Card.vue"
import FocalPoints from "./sections/FocalPoints.vue"

export default {
    name:"Main",
    components: {
        Card,FocalPoints,
    },
    data() {
        return {
            cards: [
                {name:"Languages", url:"h5-custom-icon-1.png", id:1},
                {name:"Software", url:"h5-custom-icon-2.png", id:2},
                {name:"Business", url:"h5-custom-icon-3.png", id:3},
                {name:"Chemistry", url:"h5-custom-icon-4.png", id:4},
                {name:"Science", url:"h5-custom-icon-5.png", id:5},
                {name:"DIY&Craft", url:"h5-custom-icon-6.png", id:6},
            ],
            focalPoints: [
                {text: "What We Do", url: "#", active: false},
                {text: "Degree Programme", url: "#", active: false},
                {text: "Career Achievements", url: "#", active: false},
                {text: "Personal Managment", url: "#", active: false},
                {text: "Steps To Success", url: "#", active: false},
                {text: "Knowledge Transfer", url: "#", active: false}
            ]

        }
    }
}
</script>

<style scoped lang="scss">
    .slider {
        background-image: url("../assets/img/h5-parallax-img-1.png");
    }
</style>