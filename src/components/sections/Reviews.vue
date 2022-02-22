<template>
  <section id="reviews">
    <div class="container">
        <div class="row">
            <div class="col-7">
                <!-- section image -->
                <figure class="text-center">
                    <img src="../../assets/img/h5-img-2.jpg" class="img-fluid w-75" alt="">
                </figure>
            </div>
            <div class="col-5">
                <div class="section-text">
                    <!-- Section title -->
                    <h2>Empowering Children to Reach Their Potential</h2>
                    <!-- Section text -->
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Praesentium, officia cumque adipisci ex eligendi porro doloribus! Facilis ratione sunt, obcaecati commodi excepturi odio, aut id quaerat, sequi iste laborum eveniet?</p>
                    <!-- Counter -->
                    <div id="review-counter">
                        <div class="counter">
                            <div>
                                <a href="#"><span>168</span></a>
                                <a href="#"><span>User Stories</span></a>
                            </div>
                            <div>
                                <a href="#"><span>347</span></a>
                                <a href="#"><span>Events</span></a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name:"Reviews",
}
</script>

<style scoped lang="scss">

@import "../../assets/sass/_vars.scss";

    .section-text {
        padding: 0 30px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;

        p {
            font-size: 1.1rem;
            margin-top: 1rem;
        }
    }


    .counter {
        display:flex;
        justify-content: space-between;

        div{
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-start;
            color: $main-color;
            font-weight: 500;
            margin-right: 120px;
            
        }
    }

    a:first-child {
        font-size: 4rem;
    }
    
    a:last-child {
        font-size: 1.1rem;
    }
     
</style>