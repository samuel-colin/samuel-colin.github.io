<template>
    <div class="timeline-event">
      <div class="card timeline-content">
        <div class="card-content">
          <span class="card-title activator grey-text text-darken-4">
            {{ titleJob }}
            <a v-if="id" class="btn-floating btn-small waves-effect waves-light modal-trigger grey" v-bind:href="`#${id}`"><i class="material-icons right">more_vert</i></a>
          </span>
          <p><i class="material-icons icon_alter">place</i><span>{{ subtitleJob }}</span></p>
          <p><i class="material-icons icon_alter">today</i>  <span>{{ durationJob }}</span></p>
        </div>

        <div v-if="id" v-bind:id="id" class="modal bottom-sheet">
          <div class="modal-content">
            <div class="modal-logo">
              <a :href="webSite" target="blank"><img :src="require('@/assets/' + linkImg + '')" class="circle"/></a>
            </div>
            <h4>{{ titleJob }}</h4>
            <h5><i class="material-icons icon_alter">place</i>{{ subtitleJob }}</h5>
            <h5><i class="material-icons icon_alter">today</i>  {{ durationJob }}</h5>
            <p class="modal-description" v-html="descriptionPopUp"></p>
            <p v-if="techList" class="modal-tech">
              <i class="material-icons icon_alter">settings_applications</i>
              <span v-for="techElt in techList" :key="techElt">
                <span class='tech'>{{techElt}}</span>
              </span>
            </p>
          </div>
          <div class="modal-footer">
            <a href="#!" class="modal-close waves-effect waves-green btn grey"><i class="material-icons center">navigate_next</i></a>
          </div>
        </div>
      </div>

      <div v-if="linkImg" class="timeline-badge white white-text">
        <a :href="webSite" target="blank"><img :src="require('@/assets/' + linkImg + '')" class="circle"/></a>
      </div>
      
      <div v-else class="timeline-badge white white-text"><i class="material-icons icon_alter">today</i></div>
    </div>
</template>

<script>
  export default {
    name: 'TimelineContent',
    props: {
      id: String,
      titleJob: String,
      subtitleJob: String, 
      durationJob: String, 
      descriptionPopUp: String,
      linkImg: String,
      techList: Array,
      webSite: String
    }
  }
</script>

<style scoped>
  a {
    float: right;
  }

  h5 {
    font-size: 1.5rem;
    margin-top: 0;
  }

  .icon_alter {
    vertical-align: bottom;
    margin-right: 10px;
  }

  .modal-logo img {
    height: 80px
  }

  .modal-tech {
    color: grey;
  }
  .modal-content {
    width: 700px;
    margin: 0 auto;
  }

  .modal-description {
    text-align: justify;
  }

  @media (max-width: 600px) {
    .modal-content {
      width: 100% !important;
    }
    
    .card .card-title {
      font-size: 18px;
    }

    .card .card-content {
      padding: 15px;
    }
  }
</style>