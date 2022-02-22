<template>
  <div>
      <img :src="getImageUrl(course.imageUrl)" :alt="course.name" class="img-fluid">
      <div class="card-text">
            <div class="pill rounded-pill">{{course.cost}}</div>
            <h4>{{course.name}}</h4>
            <span class="text-muted">{{course.teacher}}</span>
            <p>{{course.description}}</p>
            <div class="text-muted">
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

    .card-text {
        padding: 15px;
        position: relative;

        .pill {
            color: white;
            position: absolute;
            top:15px;
            right: 15px;
            background-color: $bg-color-yellow;
            min-width: 50px;
            text-align: center;
            font-size: 0.8rem;
        }
    }
</style>