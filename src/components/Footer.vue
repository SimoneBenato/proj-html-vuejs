<template>
  <div class="container-fluid">
    <div class="container-footer">
      <!-- sezione address -->
      <div class="left">
        <div class="address">
          <h3 class="label">Address</h3>
          <span class="description">
            382 NE 191st St # 87394 Miami, FL 33179-3899 <br>
            +1 (305) 547-9909 (9am - 5pm EST,Monday - Friday) <br>
            <a href="">support@maxcoach.com</a><br>
          </span>
          <section class="social">
            <i class="fab fa-facebook-square"></i> 
            <i class="fab fa-twitter"></i> 
            <i class="fab fa-instagram"></i> 
            <i class="fab fa-linkedin"></i> 
          </section>
        </div>
      </div>
      <div class="right">
        <!-- sezione explore -->
        <div class="explore">
          <h3 class="label">Explore</h3>
          <span class="description">
            <ul>
              <li><a href="">Start here</a></li>
              <li><a href="">Blog</a></li>
              <li><a href="">About us</a></li>
            </ul>
          </span>
        </div>
        <div>
          <span class="description">
            <br>
            <ul>
              <li><a href="">Success story</a></li>
              <li><a href="">Courses</a></li>
              <li><a href="">Contact us</a></li>
            </ul>
          </span>
        </div>
        <!-- sezione information -->
        <div class="information">
          <h3 class="label">Information</h3>
          <span class="description">
            <ul>
              <li><a href="">Membership</a></li>
              <li><a href="">Puchase guide</a></li>
              <li><a href="">Privacy policy</a></li>
              <li><a href="">Terms of service</a></li>
            </ul>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  props: {
  
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../styles/colors.scss';
.container-fluid {
  background-color: $charade;
  padding: 100px 0;

  .container-footer {
    width: 70%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;

    .label {
      color: $white;
      font-weight: bold;
      font-size: 1.7rem;
    }

    .description {
      color: $silver;
      line-height: 40px;
    }

    .social {
      color: $silver;
      font-size: 1.5rem;
      width: 200px;
      display: flex;
      justify-content: space-between;
      margin-top: 30px;
    }

    .right {
      display: flex;
      width: 40%;
      justify-content: space-between;
    }
  }
}
</style>
