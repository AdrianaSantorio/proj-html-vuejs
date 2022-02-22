<template>
  <header>
        <div class="container upper-header">
            <UpperHeader :menus="mainMenus"/>
        </div>
        <div class="background-slider" v-for="background in backgrounds" :key="background.id" :style="{'background-image': `url(${require(`../assets/img/${background.image}`)})`}"></div>
        <div class="text-element text-center">
            <h2>Contemporary Ideas</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam nulla id saepe soluta harum, suscipit aliquam vel numquam incidunt nostrum, eius quam nobis totam tempore!</p>
            <Button button-text="register now" />
        </div>
      
    </header>
</template>

<script>
import UpperHeader from "./header/UpperHeader.vue"
import Button from ".//Button.vue"
export default {
    name: "Header",
    components: {
        UpperHeader,Button,
    },
    data() {
        return {
            mainMenus: ["Home", "Courses", "Instructors", "Events", "pages", "elements"],
            backgrounds: [
                {image: "course-9-f-img.jpg" , id: 1},
                // {image: "course-2-f-img.jpg" , id: 2},
                // {image: "course-3-f-img.jpg" , id: 3},
                // {image: "course-4-f-img.jpg" , id: 4},
                // {image: "course-5-f-img.jpg" , id: 5},
                // {image: "course-6-f-img.jpg" , id: 6},
                // {image: "course-7-f-img.jpg" , id: 7},
                // {image: "course-8-f-img.jpg" , id: 8},
                // {image: "course-9-f-img.jpg" , id: 9},
            ]

        }
    }
}
</script>

<style scoped lang="scss">

    header {
        position: relative;
        color: white;

        .text-element {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%,-50%);

            h2{
                font-size: 4.5em;
            }
            p {
                font-size: 1.1em;
            }
        }
    }

    .background-slider {
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        height: 600px;
        //aggiustare l' altezza a 100%
        //aggiungere linear gradient o altra modalità di scurimento
    }

    .upper-header {
        position: absolute;
        top:0;
        left: 0;
        right: 0;
    }
</style>