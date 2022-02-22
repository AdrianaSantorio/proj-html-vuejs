<template>
  <section class="popular-courses">
        <div class="container">
            <div class="row">
            <div class="col text-center">
                <h2>Popular Online Courses</h2>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsum, ad culpa dicta error quibusdam rem obcaecati odio eum ex? Voluptate error veniam minima fugiat, explicabo temporibus ducimus aut nesciunt earum.</p>
            </div>
            </div>
            <div class="row g-4">
            <div class="col-4" v-for="(course, index) in onlineCourses" :key="index">
                <CoursesCard :course="course"/>
            </div>
      </div>

      </div>
  </section>
</template>

<script>

import CoursesCard from "./CoursesCard.vue"

export default {
 name:"PopularCourses",
 components: {
     CoursesCard,
 },
 props: ["onlineCourses"],

}
</script>

<style scoped lang="scss">

    .popular-courses {
        background-image: url("../../assets/img/page-background-img.png");
    }

    

</style>