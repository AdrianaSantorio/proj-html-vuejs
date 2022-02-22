<template>
  <main>
      <SubjectFields :cards="cards" />
      <Tutoring />
      <Reviews />
      <StudentSpotlight />
      <FocalPoints :focal-points="focalPoints" />
      <PopularCourses :online-courses="onlineCourses"/>
      <PricingPlans :options="options"/>
      <Clients :clients="clients"/>
  </main>
</template>

<script>

import SubjectFields from "./sections/SubjectFields.vue"
import Tutoring from "./sections/Tutoring.vue"
import Reviews from "./sections/Reviews.vue"
import StudentSpotlight from "./sections/StudentSpotlight.vue"
import FocalPoints from "./sections/FocalPoints.vue"
import PopularCourses from "./sections/PopularCourses.vue"
import PricingPlans from "./sections/PricingPlans.vue"
import Clients from "./sections/Clients.vue"

export default {
    name:"Main",
    components: {
        SubjectFields, Tutoring, Reviews,StudentSpotlight, FocalPoints, PopularCourses, PricingPlans, Clients,
    },
    data() {
        return {
            cards: [
                {name:"Languages", imageUrl:"h5-custom-icon-1.png", id:1},
                {name:"Software", imageUrl:"h5-custom-icon-2.png", id:2},
                {name:"Business", imageUrl:"h5-custom-icon-3.png", id:3},
                {name:"Chemistry", imageUrl:"h5-custom-icon-4.png", id:4},
                {name:"Science", imageUrl:"h5-custom-icon-5.png", id:5},
                {name:"DIY&Craft", imageUrl:"h5-custom-icon-6.png", id:6},
            ],
            focalPoints: [
                {text: "What We Do", url: "#", active: false},
                {text: "Degree Programme", url: "#", active: false},
                {text: "Career Achievements", url: "#", active: false},
                {text: "Personal Managment", url: "#", active: false},
                {text: "Steps To Success", url: "#", active: false},
                {text: "Knowledge Transfer", url: "#", active: false}
            ],
            onlineCourses: [
                {name:"Android Developer", url:"#", imageUrl:"course-5-f-img.jpg", teacher:"David Sanders", cost:"FREE", description:"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Modi aliquid non, sed nesciunt amet.", tutors:1, field:"programming" },
                {name:"Web Designing", url:"#", imageUrl:"course-6-f-img.jpg", teacher:"Jennifer Powell", cost:"FREE", description:"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Modi aliquid non, sed nesciunt amet.", tutors:1, field:"PROGRAMMING" },
                {name:"Financial Modeling", url:"#", imageUrl:"course-7-f-img.jpg", teacher:"Edward Bowman", cost:"$20", description:"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Modi aliquid non, sed nesciunt amet.", tutors:1, field:"BUSINESS" },
            ],
            clients: [
                {name:"iAcademy", url:"#", imageUrl:"h5-client-5.png"},
                {name:"Study Central", url:"#", imageUrl:"h5-client-1.png"},
                {name:"Educator", url:"#", imageUrl:"h5-client-2.png"},
                {name:"Study Central", url:"#", imageUrl:"h5-client-1.png"},
            ],
            options: [
                { description:"Number of Courses", standard:"2", professional:"4", advanced:"6"},
                { description:"Time", standard:"15 Days", professional:"30 Days", advanced:"30 Days"},
                { description:"Web Designing", standard:true, professional:true, advanced:true },
                { description:"Human Centerd Design", standard:true, professional:true, advanced:true },
                { description:"Basic Marketing", standard:false, professional:true, advanced:true },
                { description:"Python for Everybody", standard:false, professional:true, advanced:true} ,
                { description:"Android Developer", standard:false, professional:false, advanced:true },
                { description:"Business English", standard:false, professional:false, advanced:true }
            ],

        }
    }
}
</script>

<style scoped lang="scss">

</style>