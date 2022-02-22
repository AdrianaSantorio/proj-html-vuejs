<template>
  <div id="bottom-footer" class="container">
      <hr>
     <div class="flex-container">
        <div>
            <span>Copyrights 2017 &copy;Mikado Themes</span>
        </div>
        <div class="contacts">
            <span>CALL +44 300 303 0266</span>
            <span>FOLLOW US</span>
            <i class="fa-brands fa-twitter"></i>
            <i class="fa-brands fa-instagram"></i>
            <i class="fa-brands fa-facebook-f"></i>
        </div>
     </div>
  </div>
</template>

<script>
export default {
    name:"Bottom Footer",

}
</script>

<style scoped lang="scss">

@import "../../assets/sass/_mixins.scss";
@import "../../assets/sass/_vars.scss";


#bottom-footer {
    color:$t-color-m-gray;
    font-weight: 300;
}

hr {
    margin: 0;
}

.flex-container {
    
    @include flex-between;
    
    .contacts {
    
    @include flex-between;
    height: 100px;
    
        *{
            margin-left: 15px;
        }
    }
}

</style>