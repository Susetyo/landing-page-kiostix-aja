<template>
  <v-layout
    class="
    section-two
    text"
    wrap
    row>
      
      <v-flex lg6>
          <img class="container"
            src="https://www.tutorialrepublic.com/snippets/designs/thumbnail-carousel-with-content.png" />
      </v-flex>

      <v-flex 
      style="padding-left:1rem;"
      lg6>
        
        <h1 class="
          text-xs-left
          text-sm-left 
          text-md-left 
          margin-bottom-1 ">Experience</h1>
 
        <div class="
            text-xs-left 
            text-sm-left 
            text-md-left 
            margin-bottom-1 ">
          Mulai dari pentas seni dan kreasi, tuournament olahraga seminar hingga festival musik, KiosTix siap
          mendapingi event kamu dari awal hingga akhir untuk menghadirkan pengalaman event terbaik.<br />
           Mulai dari pentas seni dan kreasi, tuournament olahraga seminar hingga festival musik, KiosTix siap
          mendapingi event kamu dari awal hingga akhir untuk menghadirkan pengalaman event terbaik.<br />
           Mulai dari pentas seni dan kreasi, tuournament olahraga seminar hingga festival musik, KiosTix siap
          mendapingi event kamu dari awal hingga akhir untuk menghadirkan pengalaman event terbaik.
        </div>
      </v-flex>
  
  </v-layout>
</template>

<script>
import youtube from '~/components/Youtube.vue';

export default {
  data(){
    return{
       cards: [
        { title: 'Favorite road trips', 
          src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', 
          flex: 6 },
        { title: 'Best airlines', 
          src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', 
          flex: 6 }
      ]
    }
  },
  components: {
    youtube
  }
}
</script>

<style scoped>
  .section-two{
    margin-top: 2rem;
    /* background-image: url("https://www.w3schools.com/w3images/photographer.jpg"); */
    background-repeat: repeat;
    border-bottom: 1px solid black;
  }

  .videoWrapper {
    position: relative;
  }
  .videoWrapper iframe {
    padding: 0 45px 0 45px;  
    width: 100%;
  }

  .section-one .color-custom{ color: #ffffff;}

  .margin-bottom-1{ margin-bottom: 1rem;}
  .margin-bottom-3{ margin-bottom: 3rem;}
  .square {
    height: 75px;
    width: 75px;
  }
</style>
