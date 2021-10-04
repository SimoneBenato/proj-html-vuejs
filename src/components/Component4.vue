<template>
  <div class="container-fluid">
    <div class="container-youtube">
      <div class="video">
        <div class="logo">
          <img src="../images/icon-youtube-play.png" alt="">
        </div>
      </div>
      <div class="description">
        <div class="title">
          <h2>To Thrive In Business Today, You'll Need a Good Plan</h2>
          <div class="faq">
            <h3>How can we help?</h3>
            <p>How many courses you've been on, using however many techniques and methods. Unless you've come to realize the value of mindset, then you've yet to understand how success comes.</p>
            <p>With everyone else's mindset involved impacting too. Hence why business coaching is so crucial for success.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Component4',
  props: {                                                 
  
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../styles/colors.scss';
.container-fluid {
  width: 100%;
  background-color: $tuna;
  background-image: url('../images/background-map-dots-top-right-transparent.png');
  background-size: contain;
  
  .container-youtube {
    display: flex;
    width: 80%;
    margin: 0 auto;
    align-items: center;
    height: 75vh;
    justify-content: space-evenly;

    .video {
      height: 400px;
      width: 595px;
      background-image: url('../images/home-business-video-poster-670x450.jpg');
      background-size: contain;
      background-repeat: no-repeat;
      border-radius: 10px;
      position: relative;
    }

    .logo {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }

    .description {
      width: 500px;
      height: 470px;
      border-bottom: 1px solid $silver;

      .title {
        text-align: start;
        h2 {
          color: $white;
        }
        p {
          color: $white;
          margin: 20px auto;
        }
      }
    }
  }
} 
</style>
