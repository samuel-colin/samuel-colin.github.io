<template>
  <HeaderCV />
  
  <div class="col s12 m8 offset-m2 l6 offset-l3">
    <div class="row valign-wrapper">
      <div class="col l3 m0"></div>
      <div class="col l6 m12 card-panel grey lighten-5 z-depth-2">
        <ProfessionalExperiences />
      </div>
      <div class="col l3 m0"></div>
    </div>
  </div>


  <div class="col s12 m8 offset-m2 l6 offset-l3">
    <div class="row valign-wrapper">
      <div class="col l3 m0"></div>
        <div class="col l6 m12 card-panel grey lighten-5 z-depth-2">
        <EducationCV />
      </div>
      <div class="col l3 m0"></div>
    </div>
  </div>
</template>

<script>
import HeaderCV from './components/HeaderCV.vue'
import ProfessionalExperiences from './components/ProfessionalExperiences.vue'
import EducationCV from './components/EducationCV.vue'
import M from 'materialize-css'


export default {
  name: 'App',
  components: {
    HeaderCV,
    ProfessionalExperiences,
    EducationCV
  },
  mounted () {
    M.AutoInit()
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 10px;
  background-color: darkgoldenrod;
}

@import '@/styles/timeline.css';
</style>
