<template>
  <div class="upper-footer container">
      <!-- Footer Menu -->
      <div class="row">
          <div class="col-8">
              <div class="row">
                  <!-- CONTACTS -->
                  <div class="col-4">
                      <!-- Logo -->
                      <a href="#"><img src="../../assets/img/footer-logo-1.png" alt="#" class="img-fluid"></a>
                      <p>Providing Life Changing Experiences Through Education. Class That Fit Your Busy Life. Closer to Home</p>
                      <!-- contacts -->
                      <div class="d-flex flex-column text-white">
                          <span><i class="fa-solid fa-phone"></i> 1-677-124-44227</span>
                            <span><i class="fa-regular fa-clock"></i>Mon - Sat 8.00 - 18.00</span>
                      </div>
                  </div>
                <!-- COURSES -->
                  <div class="col-4">
                      <h4>Popular Courses</h4>
                      <ul>
                          <li>
                            <a href="#"><h6>Business English</h6></a>
                            <a href="#"><span>Preston Marshall</span></a>
                          </li>
                          <li>
                            <a href="#"><h6>Social Computing</h6></a>
                            <a href="#"><span>David Sanders</span></a>
                          </li>
                          <li>
                            <a href="#"><h6>Learn Spanish</h6></a>
                            <a href="#"><span>Jennie King</span></a>
                          </li>
                        </ul>
                  </div>
                  <!-- SUPPORT -->
                  <div class="col-4">
                      <h4>Support</h4>
                      <ul>
                          <li><a href="#">User Dashboard</a></li>
                          <li><a href="#">Contact Us</a></li>
                          <li><a href="#">FAQ</a></li>
                          <li><a href="#">Course Offer</a></li>
                          <li><a href="#">Events</a></li>
                      </ul>
                  </div>
              </div>
          </div>
          <div class="col-4 text-center">
              <!-- Footer image -->
              <h4> Flexible Learning</h4>
              <figure>
                  <a href="#"><img src="../../assets/img/footer-img-1.png" alt="Branches" class="img-fluid w-75"></a>
                  </figure>
          </div>
      </div>
  </div>
</template>

<script>

export default {
name: "Upper Footer",
}
</script>

<style scoped lang="scss">

    @import "../../assets/sass/_vars.scss";

    .upper-footer {
        color:$t-color-off-white;
        padding: 40px 0;
    }

    ul {
        padding:0;

        li {
            margin-bottom: 15px;
        }
    }

    h4 {
        color: white;
    }

    h6 {
        color: $t-color-off-white;
    }

    p {
        font-weight: 100;
        margin: 15px 0;
    }
</style>