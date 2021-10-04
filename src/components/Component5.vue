<template>
  <div class="container">
    <!-- sezione descrittiva dei vari servizi offerti -->
    <div class="description title">
      <h3>Wanna transform your life?</h3>
      <h2>Upcoming Events</h2>
    </div>

    <!-- sezione offerte -->
    <div class="features-container">
      <div class="features" v-for="(item, index) in features" :key="index">
        <div>
          <span class="position"><i class="fas fa-map-marker-alt"></i> {{item.position}}</span><br>
          <span class="title">{{item.title}}</span>
        </div>
        <div class="get-ticket">
          <span>
            <span class="date">{{item.date}}</span><br>
            {{item.month}}
          </span>
          <button class="green">Get Ticket</button>
        </div>
      </div>
    </div>

    <div class="all-courses">
      <p>Excited about our event? <span><a href="">View all events  <i class="fas fa-long-arrow-alt-right"></i></a></span></p>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Component1',
  props: {                                                 
  
  },
  data() {
    return {
      features: [
      {
          title: 'Storytelling Workshop',
          position: 'Texas, US',
          date: '22',
          month: 'NOV',
      },
      {
          title: 'Painting Art Contest 2020',
          position: 'New Yorck, US',
          date: '10',
          month: 'OCT',
      },
      {
          title: 'International Art Fair 2020',
          position: 'Hamburg, Germany',
          date: '23',
          month: 'NOV',
      },
      {
          title: 'Street Performance: Call for Artist',
          position: 'Illinois, US',
          date: '15',
          month: 'DEC',
      },
      {
          title: 'Consumer Food Safety Education Conference',
          position: 'Illinois, US',
          date: '22',
          month: 'JUL',
      },
      {
          title: 'How meditation improve your mental health?',
          position: 'Dubai',
          date: '12',
          month: 'AUG',
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
  width: 70%;
  
  .description {
    width: 70%;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  
  .features-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    
    .features {
      width: calc((100% / 2) - 30px);
      display: flex;
      margin: 15px auto;
      height: 150px;
      justify-content: space-between;
      padding: 20px;
      background-color: $porcelain;
      
      .title {
        font-size: 2.3rem;
      }

      .position {
        color: $boulder;
      }

      .get-ticket {
        display: flex;
        flex-direction: column;
        align-items: center;
      
        .date {
          font-size: 2.5rem;
          color: $jungle_green;
        }
  
        button {
          padding: 10px;
          border-radius: 10px;
          width: 100px;
          margin: 10px;
          }
  
        .green {
          background-color: $mountain_meadow;
          color: $white;
        }
      }
    }
  }

  .all-courses {
    text-align: center;
    font-size: 1.5rem;
    color: $boulder;

    a {
      color: $jungle_green;
    }
  }
}
</style>
