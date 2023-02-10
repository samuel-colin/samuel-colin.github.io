<template>
  <header class="col s12 m8 offset-m2 l6 offset-l3">
    <div class="card-panel grey lighten-4 z-depth-2">
      <div class="row valign-wrapper">
        <div class="col l2 m0">
        </div>
        <div class="col l2 m2">
          <img src="@/assets/photo_profil_circle.jpeg" alt="" class="circle responsive-img">
        </div>
        <div class="col l6 m8">
          <h1>Samuel Colin</h1>
          <h2>Ingénieur Informatique chez Younup</h2>
          <h3>Lyon (69), France</h3>
          <div class="social">
            <a href="https://github.com/samuel-colin" target="blank"><img src="@/assets/icon_github.png"/></a>
            <a href="https://www.linkedin.com/in/colin-samuel/" target="blank"><img src="@/assets/icon_linkedin.png"/></a>
            <a href="https://twitter.com/samuel_c0l1" target="blank"><img src="@/assets/icon_twitter.png"/></a>
            <a href="https://stackoverflow.com/users/3455763/samuel" target="blank"><img src="@/assets/icon_stackoverflow.png"/></a>
          </div>
        </div>
        <div class="col l2 m0">
        </div>
      </div>
    </div>
  </header>

</template>

<script>
  export default {
    name: 'HeaderCV'
  }
</script>

<style scoped>
  h1 {
    font-size: 5rem !important;
  }

  h2 {
    font-size: 2rem !important;
    margin-bottom: 10px;
    margin-top: 0;
  }

  h3 {
    font-size: 1rem !important;
    margin-top: 0;
  }

  .social img {
    width: 30px;
    margin-right: 10px;
  }

  @media (max-width: 800px) {
    h1 {
      font-size: 2.5rem !important;
      margin-top: 10px;
    }

    h2 {
      font-size: 1.2rem !important;
    }

    h3 {
      font-size: 1rem !important;
      margin-top: 0;
    }

    .card-panel {
      height: 250px !important;
      padding: 0;
    }
    
    img.responsive-img {
      max-width: 150px !important;
      height: 20% !important;
    }

    .col .row {
      margin-left: 0;
      margin-right: 0;
    }
  }
</style>