<template>
    <nav class="h-100">
        <ul>
            <li v-for="(link, index) in links" :key="index" :class="{active: link.active}" @mouseover="isActive(true,index)" @mouseleave="isActive(false,index)">
                <a :href="link.url">{{link.text}}</a>              
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: "Vertical Navbar",
    props: ["links"],
    methods: {
        isActive(status, index) {
            this.links[index].active = status;
        }
    }
}
</script>

<style scoped lang="scss">

@import "../../assets/sass/_vars.scss";

    nav ul {
        display: flex;
        flex-direction: column;
        height: 100%;
        margin: 0;
        padding: 0;
        border-left: 1px solid $b-color-l-grey;
        border-top: 1px solid $b-color-l-grey;
        border-right: 1px solid $b-color-l-grey;

        li {
            display: flex;
            align-items: flex-start;
            list-style-type: none;
            border-bottom: 1px solid $b-color-l-grey;
            border-left:6px solid transparent;
            margin-top: -1px;
            padding: 15px;
            color: #ABABAB;

            a{
            font-weight: 600;
            font-size: 1rem;

            &:hover {
                color: inherit;
            }
            }

            &.active {
                color: $main-color;
                border-left: 6px solid $main-color;
            }
        }
    }

</style>