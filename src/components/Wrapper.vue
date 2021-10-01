<template>
  <div class="container-fluid">
    <div class="container-wrapper">
      <!-- sezione scritte -->
      <div class="click-bait">
        <h3>New Challenges, New Skills</h3>
        <h1>BUILD YOUR OWN LIFE COACHING BUSINESS</h1>
        <p>Whole-Life Business Coaching for committed entrepreneurs</p>
        <button>Get started today</button>
      </div>
      <!-- sezione immagini -->
      <div class="image">
        <img src="../images/home-business-hero-avatar.png" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Wrapper',
  props: {
  
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../styles/colors.scss';
.container-fluid {
  width: 100%;
  background-color: $porcelain;
  height: calc(100vh - 50px);
  position: relative;
  
  .container-wrapper {
    width: 80%;
    margin: 0 auto;
    display: flex;
    height: 100%;
  
    .click-bait {
      width: 40%;
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 150px;

      h3 {
        color: $jungle_green;
        margin-bottom: 20px;
      }

      h1 {
        color: $charade;
        margin-bottom: 20px;
      }

      p {
        color: $boulder;
        margin-bottom: 20px;
      }

      button {
        background-color: $mountain_meadow;
        color: $white;
        padding: 10px;
        border-radius: 10px;
        width: 150px;
      }
    }

    .image {
      width: 60%;
      background-image: url('../images/home-business-hero-global-image.png');
      background-size: cover;
      height: 100%;
      position: relative;

      img {
        position: absolute;
        bottom: 0;
        right: 10%;
      }
    }
  }

}
</style>
