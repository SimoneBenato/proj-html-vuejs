<template>
  <div class="container-fluid">
    <div class="container">
      <div class="title">
        <h3>Let's Dream Big Together</h3>
        <h2>Explore How can i help you</h2>
      </div>
      <!-- sezione delle carte -->
      <div class="card-section">
        <div class="card">
          <div class="img">
            <img src="../images/home-business-service-slide-01-480x298.jpg" alt="">
          </div>
          <div class="description">
            <h4>Consultative Training</h4>
            <p>With a coach addressing multiple issues that are off balance, affecting your business in various unconsidered ways.</p>
          </div>
          <div class="link">
            <a href="">
              <span>Discover now <i class="fas fa-long-arrow-alt-right"></i></span>
            </a>
          </div>
        </div>
        <div class="card">
          <div class="img">
            <img src="../images/home-business-service-slide-02-480x298.jpg" alt="">
          </div>
          <div class="description">
            <h4>Real Deal Coaching</h4>
            <p>Brings an exceptionally powerful opportunity. Being able to accept, to work with that opportunity.</p>
          </div>
          <div class="link">
            <a href="">
              <span>Discover now <i class="fas fa-long-arrow-alt-right"></i></span>
            </a>
          </div>
        </div>
        <div class="card">
          <div class="img">
            <img src="../images/home-business-service-slide-03-480x298.jpg" alt="">
          </div>
          <div class="description">
            <h4>Advisor Training Program</h4>
            <p>Getting High quality, entrepreneur mindset driven online business coaching, is what is needed</p>
          </div>
          <div class="link">
            <a href="">
              <span>Discover now <i class="fas fa-long-arrow-alt-right"></i></span>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Component2',
  props: {                                                 
  
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../styles/colors.scss';
.container-fluid {
  width: 100%;
  background-color: $porcelain;
  

  .container {
    width: 80%;

    .card-section {
      display: flex;
      justify-content: center;

      .card {
      width: calc((90% / 3) - 20px);
      height: 500px;
      margin-right: 20px;
      background-color: $white;
      border-radius: 10px;

        .img {
          height: 50%;

          img {
            width: 100%;
            height: 100%;
            border-top-right-radius: 10px;
            border-top-left-radius: 10px;
          }
        }

        .description {
          height: 40%;
          padding: 40px;

          h4 {
            font-size: 2rem;
            margin-bottom: 15px;
          }

          p {
            font-size: 1.1rem;
            color: $boulder;
          }
        }

        .link {
          height: 10%;
          border-top: 1px solid $porcelain;
          font-weight: bold;
          font-size: 1.2rem;
          display: flex;
          justify-content: center;
          align-items: center;

          a {
            color: $jungle_green;
          }
        }
      }
    }
  }
} 
</style>
