<template>
  <div class="course-card">
      <img :src="getImageUrl(course.imageUrl)" :alt="course.name" class="img-fluid">
      <div class="card-text">
            <div class="pill rounded-pill" :class="course.free ? 'bg-yellow' : 'bg-blue'">{{course.cost}}</div>
            <!-- course name -->
            <h5>{{course.name}}</h5>
            <!-- teacher name -->
            <span>{{course.teacher}}</span>
            <!-- course description -->
            <p>{{course.description}}</p>
            <div class="tags">
                <span><i class="fa-solid fa-user"></i>{{course.tutors}}</span>
                <span><i class="fa-solid fa-tag"></i>{{course.field}}</span>
            </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"Courses Card",
    props:["course"],
    methods: {
        getImageUrl(imageUrl) {
            return require(`../../assets/img/${imageUrl}`);
        
        }
    }
}
</script>

<style scoped lang="scss">

    @import "../../assets/sass/_vars.scss";

    .course-card {
        border: 1px solid $b-color-l-grey;

        .tags {
            * {
                margin-right: 15px;
            }
        }
    }

    .card-text {
        padding: 15px;
        position: relative;
        color: $t-color-gray;

        .pill {
            color: white;
            position: absolute;
            top:15px;
            right: 15px;       
            min-width: 50px;
            text-align: center;
            font-size: 0.8rem;

            &.bg-yellow {
                background-color: $bg-color-yellow;
            }

            &.bg-blue {
                background-color: $main-color;
            }
        }
    }
</style>