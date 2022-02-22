<template>
  <section id="student-spotlight">
        <div class="slider container">
            <div class="slider-content text-center">
                <!-- img -->
                <div class="student-picture"></div>
                <!-- text -->
                <p>"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tenetur labore minus quam repudiandae quas iure! Voluptatibus nulla veniam, iure culpa maxime ullam illum laborum nemo, reprehenderit dicta repellat neque quo."</p>
                <!-- name -->
                <h4>Joan Collins</h4>
                <!-- role -->
                <span>STUDENT</span>        
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:"Student Spotlight",
}
</script>

<style scoped lang="scss">

@import "../../assets/sass/_vars.scss";

#student-spotlight {
    padding: 150px 200px;
    color: white;
    background-image: url("../../assets/img/h5-parallax-img-1.png");
    background-position: top;
    background-size: 140%;

    .student-picture {
        border-radius:50%;
        overflow: hidden;
        background-image: url("../../assets/img/instructor-img-6.jpg");
        background-position: top;
        background-size: 150%;

        width: 100px;
        height: 100px;
        margin: 30px auto;
    }

    h4 {
        color: white;
    }

    p {
        font-size:1.3rem;
        font-weight: 300;
        margin: 40px 0;
    }
    
}

</style>