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
            <span>Discover now <i class="fas fa-long-arrow-alt-right"></i></span>
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
            <span>Discover now <i class="fas fa-long-arrow-alt-right"></i></span>
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
            <span>Discover now <i class="fas fa-long-arrow-alt-right"></i></span>
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
      margin-top: 50px;

      .card {
      width: calc((100% / 3) - 20px);
      height: 600px;
      margin-right: 20px;
      background-color: $white;
      border-radius: 25px;

        .img {
          height: 50%;

          img {
            width: 100%;
            border-top-right-radius: 25px;
            border-top-left-radius: 25px;
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
            font-size: 1.3rem;
            color: $boulder;
          }
        }

        .link {
          height: 10%;
          border-top: 1px solid $porcelain;
          color: $jungle_green;
          font-weight: bold;
          font-size: 1.2rem;
          display: flex;
          justify-content: center;
          align-items: center;
        }
      }
    }
  }
} 
</style>
