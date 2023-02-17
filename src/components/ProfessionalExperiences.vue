<template>
  <h1>Expériences Professionnelles</h1>

  <div class="timeline">
    <!-- YOUNUP -->
    <TimelineContent 
      id="younupModal"
      titleJob="Ingénieur Informatique"
      subtitleJob="Younup - Lyon (69)"
      durationJob="De Janvier 2023 à aujourd'hui"
      descriptionPopUp="Développeur BackEnd sur le projet interne Younup GreenMorrow (Reconnaissance de plantes via une IA)"
      linkImg="logo_younup.png"
      techList="<span class='tech'>Java</span>
        <span class='tech'>JEE</span></span>
        <span class='tech'>Spring Boot</span>
        <span class='tech'>Vue.JS</span>
        <span class='tech'>Angular</span>
        <span class='tech'>NodeJS</span>
        <span class='tech'>Junit (Tests Unitaires)</span>"
    />

    <!-- ADVENTIEL -->
    <TimelineContent 
      id="adventiel1Modal"
      titleJob="Lead Dev"
      subtitleJob="Adventiel - Rennes (35)"
      durationJob="De Septembre 2019 à Janvier 2023"
      descriptionPopUp="Lead Dev sur le projet <a href='https://idele.fr/detail-article/cap2err' alt='Site CAP2ER'>CAP2ER</a> pour le client <a href='https://idele.fr/' alt='Site IDELE'>IDELE</a>. 
        <br/>Au sein d'une équipe de 10 psonnes, mon rôle était d'accompagner l'équipe techniquement et fonctionnellement et d'être référent."
      linkImg="logo_adventiel.jpg"
      techList="<span class='tech'>Java</span>
        <span class='tech'>JEE</span>
        <span class='tech'>Spring Boot</span>
        <span class='tech'>BDD PostgreSQL</span>
        <span class='tech'>BackboneJS</span>
        <span class='tech'>Junit (Tests Unitaires)</span>
        <span class='tech'>Mockito (Tests d'intégration)</span>"
    />, 

    <!-- ADVENTIEL -->
    <TimelineContent 
      id="adventiel2Modal"
      titleJob="Développeur Confirmé"
      subtitleJob="Adventiel - Rennes (35)"
      durationJob="De Septembre 2019 à Janvier 2023"
      descriptionPopUp="Je suis intervenu sur différents projets pour des clients du monde de l'Agriculture et de l'Agroalimentaire (SARIA, ATEMAX, DENKAVIT et INNOVAL)."
      linkImg="logo_adventiel.jpg"
      techList="<span class='tech'>Java</span>
        <span class='tech'>JEE</span>
        <span class='tech'>Spring Boot</span>
        <span class='tech'>Liferay</span>
        <span class='tech'>Envox</span>
        <span class='tech'>BDD PostgreSQL</span>
        <span class='tech'>BDD Oracle</span>"
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
      techList="<span class='tech'>Java</span>
        <span class='tech'>JEE</span>
        <span class='tech'>Angular JS</span>
        <span class='tech'>Angular 4</span>
        <span class='tech'>NodeJS</span>"
    />

    <!-- ASI -->
    <TimelineContent 
      id="asi1Modal"
      titleJob="Scrum Master & Ingénieur Java JEE"
      subtitleJob="ASI - Brest (29)"
      durationJob="De Mars 2017 à Février 2018"
      descriptionPopUp="Dans le cadre de la création de la néo-banque 'Au max' par le Crédit Mutuel Arkéa, j'ai eu le rôle de ScrumMaster et de développeur au sein d'une des équipes Back-End."
      linkImg="logo_asi.jpg"
      techList="<span class='tech'>Java</span>
        <span class='tech'>JEE</span>
        <span class='tech'>Spring Boot</span>
        <span class='tech'>Méthodologie Agile</span>
        <span class='tech'>Microservices</span>
        <span class='tech'>REST API</span>"
    />

    <!-- Sopra Stéria -->
    <TimelineContent 
      id="sopra2Modal"
      titleJob="Ingénieur Java JEE"
      subtitleJob="Sopra Stéria - Rennes (35)"
      durationJob="De Juillet 2015 à Décembre 2016"
      descriptionPopUp="Développements Back-End Java JEE sur un outil de gestion de situations stratégiques pour un client du secteur public."
      linkImg="logo_soprasteria.jpg"
      techList="<span class='tech'>Java</span>
        <span class='tech'>JEE</span>
        <span class='tech'>Spring</span>
        <span class='tech'>Maven</span>
        <span class='tech'>Angular JS</span>
        <span class='tech'>Jenkins</span>"
    />  

    <!-- Sopra Stéria -->
    <TimelineContent 
      id="sopra1Modal"
      titleJob="Ingénieur Développement"
      subtitleJob="Sopra Stéria - Rennes (35)"
      durationJob="De Septembre 2013 à Juin 2015"
      descriptionPopUp="Développements divers sur des outils internes ou pour des clients du secteur public."
      linkImg="logo_soprasteria.jpg"
      techList="<span class='tech'>Python</span>
        <span class='tech'>BPMN 2.0</span>
        <span class='tech'>Angular JS</span>
        <span class='tech'>Microsoft PowerShell</span>
        <span class='tech'>Microsoft SharePoint API</span>
        <span class='tech'>Java</span>
        <span class='tech'>JEE</span>"
    />

    <!-- CGI -->
    <TimelineContent 
      id="cgiModal"
      titleJob="Ingénieur Oracle Application"
      subtitleJob="CGI - Brest (29)"
      durationJob="De Avril 2012 à Août 2013"
      descriptionPopUp="Développements dans le cadre d’une migration de version d’un ERP Oracle Application."
      linkImg="logo_cgi.jpg"
      techList="<span class='tech'>Base de données Oracle</span>
        <span class='tech'>PL/SQL</span>
        <span class='tech'>environnements Linux</span>"
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