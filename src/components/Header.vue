<template>
  <div class="container-header">
    <!-- logo -->
    <div class="logo">
      <a href="">
        <img src="../images/dark-logo.png" alt="">
      </a>
    </div>
    <!-- menù di navigazione -->
    <nav>
      <ul class="links">
        <li>
          <a href="">
            Home <i class="fas fa-chevron-down"></i>
          </a>
        </li>
        <li>
          <a href="">
            Pages <i class="fas fa-chevron-down"></i>
          </a>
        </li>
        <li>
          <a href="">
            Courses <i class="fas fa-chevron-down"></i>
          </a>
        </li>
        <li>
          <a href="">
            Features <i class="fas fa-chevron-down"></i>
          </a>
        </li>
        <li>
          <a href="">
            Blog <i class="fas fa-chevron-down"></i>
          </a>
        </li>
        <li>
          <a href="">
            Shop <i class="fas fa-chevron-down"></i>
          </a>
        </li>
      </ul>
    </nav>
    <!-- selezione lingua sito -->
    <div class="leng_serch">
      <div class="leng">
        <img src="../images/en.png" alt="">
        <a href="">
          <p>ENGLISH <i class="fas fa-chevron-down"></i></p>
        </a>
        <a href="">
          <i class="far fa-user-circle"></i>
        </a>
      </div>

    <!-- barra di ricerca -->
      <div>
        <input type="text" name="" id="" placeholder="Serch...">
        <a href="">
          <i class="fas fa-search"></i>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 50px;
  width: 100%;

  .logo {
    width: 320px;

    img {
      width: 40%;
      margin-left: 120px;
    }
  }

  .links {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 600px;

    i {
      font-size: 0.5rem;
    }
  }

  .leng_serch{
    margin-right: 20px;
    display: flex;
    align-items: center;

    .leng {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 150px;
      margin-right: 10px;

      p {
        font-size: 0.8rem;
      }
    }

    input {
    height: 50px;
    padding: 10px;
    border: none;
  }
  }
  
}
</style>
