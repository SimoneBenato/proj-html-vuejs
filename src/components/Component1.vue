<template>
  <div class="container">
    <!-- sezione descrittiva dei vari servizi offerti -->
    <div class="description title">
      <h3>Let's Dream Big Together</h3>
      <p>We are pioneers of the digital approach, using leading-edge technology to simplify procedures and apply executive coaching in the new age of digitalization.</p>
    </div>

    <!-- sezione offerte -->
    <div class="features">
      <h5></h5>
      <p></p>
    </div>

    <!-- sezione pulsanti -->
    <div class="btn-section">
      <button class="white">Learn More</button>
      <button class="green">Get Started Today</button>
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
          title: 'One to One',
          description: 'Getting the necessary clarity about the current state to help you improve your game'
      },
      {
          title: 'Anywhere',
          description: 'Access to valuable and portable program which allow you  to setup and live anywhere you want'
      },
      {
          title: 'On Time',
          description: 'Punctuality is our top priority because it is an essential criteria to assess a program quality.'
      },
      {
          title: 'Online Coures',
          description: 'Online business coaching noe offers you a very powerful way to empower your business into success.'
      },
      {
          title: 'Consulting',
          description: 'You will get a clear sense of direction for your business, thorought assessment and faster results.'
      },
      {
          title: 'Self Development',
          description: 'Business Coaching often keep your focus and develop you both in a professional and personal way.'
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
  width: 80%;
  
  .description {
    width: 70%;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    justify-content: center;

    p {
      font-size: 2.5rem;
      margin: 50px auto;
    }
  }
  
  .features {
    width: calc(100% / 3);
    padding: 20px;

    h5 {
      font-size: 1.8rem;
      margin-bottom: 15px;
      color: $charade;
    }

    p {
      font-size: 1.3rem;
      color: $boulder
    }
  }

  .btn-section {
    display: flex;
    justify-content: center;

     button {
        padding: 10px;
        border-radius: 10px;
        width: 150px;
        margin: 10px;
        }

      .green {
        background-color: $mountain_meadow;
        color: $white;
      }

      .white {
        background-color: $white;
        color: $mountain_meadow;
      }
      
  }
}
</style>
