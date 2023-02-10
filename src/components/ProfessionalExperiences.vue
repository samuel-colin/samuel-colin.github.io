<template>
  <h1>Expériences Professionnelles</h1>

  <div class="timeline">
    <!-- YOUNUP -->
    <TimelineContent 
      id="younupModal"
      titleJob="Ingénieur Informatique"
      subtitleJob="Younup - Lyon (69)"
      durationJob="De Janvier 2023 à aujourd'hui"
      descriptionPopUp=""
      linkImg="logo_younup.png"
      techList="Java, JEE, Spring Boot, Vue.JS, Angular, NodeJS"
    />

    <!-- ADVENTIEL -->
    <TimelineContent 
      id="adventielModal"
      titleJob="Développeur Confirmé"
      subtitleJob="Adventiel - Rennes (35)"
      durationJob="De Septembre 2019 à Janvier 2023"
      descriptionPopUp="=> Je suis intervenu sur différents projets pour des clients du monde de l'Agriculture et de l'Agroalimentaire.  
        <br/>=> J'ai également été Lead Dev dans une équipe de 8 personnes. Mon rôle était d'accompagner les profils plus juniors et d'être référent sur la partie technique et fonctionnelle."
      linkImg="logo_adventiel.jpg"
      techList="Java, JEE, Spring Boot, Liferay, Envox"
    />

    <!-- ASI -->
    <TimelineContent 
      id="asi2Modal"
      titleJob="Concepteur Réalisateur"
      subtitleJob="ASI - Rennes (35)"
      durationJob="De Mars 2018 à Aout 2019"
      descriptionPopUp="J'ai été Concepteur Réalisateur dans le cadre de plusieurs projets de TMA dans l'environnement technique JEE.
        <br/> J'ai été également été Développeur pour un progiciel de la société <a href='https://www.mgdis.fr/' alt='MGDIS'>MGDIS</a>. "
      linkImg="logo_asi.jpg"
      techList="Java, JEE, Angular JS, Angular 4, NodeJS"
    />

    <!-- ASI -->
    <TimelineContent 
      id="asi1Modal"
      titleJob="Scrum Master & Ingénieur Java JEE"
      subtitleJob="ASI - Brest (29)"
      durationJob="De Mars 2017 à Février 2018"
      descriptionPopUp="Dans le cadre de la création de la néo-banque 'Au max' par le Crédit Mutuel Arkéa, j'ai eu le rôle de ScrumMaster et de développeur au sein d'une des équipes Back-End."
      linkImg="logo_asi.jpg"
      techList="Java, JEE, Spring Boot, Méthodologie Agile, Microservices, REST API"
    />

    <!-- Sopra Stéria -->
    <TimelineContent 
      id="sopra2Modal"
      titleJob="Ingénieur Java JEE"
      subtitleJob="Sopra Stéria - Rennes (35)"
      durationJob="De Juillet 2015 à Décembre 2016"
      descriptionPopUp="Développements Back-End Java JEE sur un outil de gestion de situations stratégiques pour un client du secteur public."
      linkImg="logo_soprasteria.jpg"
      techList="Java, JEE, Spring, Maven, Angular JS, Jenkins"
    />  

    <!-- Sopra Stéria -->
    <TimelineContent 
      id="sopra1Modal"
      titleJob="Ingénieur Développement"
      subtitleJob="Sopra Stéria - Rennes (35)"
      durationJob="De Septembre 2013 à Juin 2015"
      descriptionPopUp="Développements divers sur des outils internes ou pour des clients du secteur public."
      linkImg="logo_soprasteria.jpg"
      techList="Python, BPMN 2.0, Angular JS, Microsoft PowerShell, Microsoft SharePoint API, Java, JEE"
    />

    <!-- CGI -->
    <TimelineContent 
      id="cgiModal"
      titleJob="Ingénieur Oracle Application"
      subtitleJob="CGI - Brest (29)"
      durationJob="De Avril 2012 à Août 2013"
      descriptionPopUp="Développements dans le cadre d’une migration de version d’un ERP Oracle Application."
      linkImg="logo_cgi.jpg"
      techList="Base de données Oracle, PL/SQL, environnements Linux"
    />
  </div>
</template>

<script>
import TimelineContent from '@/components/TimelineContent.vue'

  export default {
    name: 'ProfessionalExperiences',
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