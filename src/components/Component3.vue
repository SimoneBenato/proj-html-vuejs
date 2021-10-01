<template>
  <div class="container">
    <div class="title">
      <h3>Let's Dream Big Together</h3>
      <h2>Explore How can i help you</h2>
    </div>

    <div class="card-section">
      <div class="card" v-for="(item, index) in courses" :key="index" :style="{'background-image': 'url(' + require('../images/' + item.image) + ')'}">
        <span class="price">{{item.price}}</span>
        <p class="service">{{item.service}}</p>
      </div>
    </div>

    <div class="links">
      <p>Take the control of their life back and start doing things to make their dream come true.<span class="bold">View all courses <i class="fas fa-long-arrow-alt-right"></i></span></p>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Component3',
  props: {                                                 
  
  },
  data() {
    return {
      courses: [
        {
            price: '$40.00',
            service: 'Learn to Write as a Professional Author',
            image: 'course-02-443x600.jpg'
        },
        {
            price: 'Free',
            service: 'Customer-centric Info-Tech Strategies',
            image: 'stock-full-hd-03-443x600.jpg'
        },
        {
            price: '$19.00',
            service: 'Open Programming Courses for Everyone: Python',
            image: 'stock-full-hd-04-443x600.jpg'
        },
        {
            price: '$26.00',
            service: 'Academic Listening and Note-taking',
            image: 'stock-full-hd-06-443x600.jpg'
        }
      ]
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../styles/colors.scss';
.container {
  width: 90%;

  .card-section {
    display: flex;
    justify-content: space-evenly;

    .card {
      width: calc((100% / 4) - 40px);
      height: 500px;
      // background-image: url('../images/course-02-443x600.jpg');
      border-radius: 10px;
      padding: 30px;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;

      .price {
        color: $jungle_green;
        font-size: 1.7rem;
        font-weight: bold;
      }

      .service {
        color: $white;
        font-size: 2rem;
        font-weight: bold;
      }
    }
  }

  .links {
    text-align: center;
    font-size: 1.3rem;
    width: 30%;
    margin: 0 auto;
    color: $boulder;

    .bold {
      font-weight: bold;
      color: black;
    }
  }
}
</style>
