<template>
  <h1>Formation</h1>

  <div class="timeline">
    <!-- MOOC -->
    <TimelineContent 
      titleJob="MOOC SecNumacadémieMOOC"
      subtitleJob="ANSSI - Agence nationale de la sécurité des systèmes d'information"
      durationJob="2020"
      linkImg="logo_anssi.png"
    />

    <!-- Master -->
    <TimelineContent 
      titleJob="Master en Ingénierie Informatique"
      subtitleJob="Université de Bretagne Occidentale - Brest (29)"
      durationJob="2013"
      linkImg="logo_ubo.png"
    />

    <!-- Licence -->
    <TimelineContent 
      titleJob="Licence Informatique"
      subtitleJob="Université d'Angers (49)"
      durationJob="2011"
      linkImg="logo_ua.png"
    />

    <!-- Baccalauréat -->
    <TimelineContent 
      titleJob="Baccalauréat Economique et Sociale, option Mathématiques"
      subtitleJob="Lycée Blaise Pascal - Segré (49)"
      durationJob="2008"
      linkImg="logo_school.png"
    />
  </div>
</template>

<script>
import TimelineContent from '@/components/TimelineContent.vue'

  export default {
    name: 'EducationCV',
    components: {
      TimelineContent
    }
  }
</script>

<style scoped>
  h1 {
    font-size: 2rem;
    color: grey;
  }

    
  @media (max-width: 800px) {
    h1 {
      font-size: 1.5rem;
      margin-top: 1rem;
    }
  }
</style>