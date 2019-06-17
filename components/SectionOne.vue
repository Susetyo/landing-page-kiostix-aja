<template>
  <v-layout
    class="section-one"
    wrap
    row>
      
      <v-flex lg12>
        <h1 class="
            text-xs-center 
            text-sm-center 
            text-md-center 
            margin-bottom-1 
            color-custom">#KiosTixAja!</h1>
      </v-flex>

      <v-flex  
        offset-md4
        md4>
        <div class="
            text-xs-center 
            text-sm-center 
            text-md-center 
            margin-bottom-1 
            color-custom">
          Mulai dari pentas seni dan kreasi, tuournament olahraga seminar hingga festival musik, KiosTix siap
          mendapingi event kamu dari awal hingga akhir untuk menghadirkan pengalaman event terbaik.
        </div>
      </v-flex>
      
      <v-flex lg12>
        <div
          class="
            videoWrapper 
            text-xs-center 
            text-sm-center 
            text-md-center 
            margin-bottom-1">
          <youtube 
            width="800"
            height="700"
            :yid="videoId"/>
        </div>
      </v-flex>

      <v-flex lg12>
        <h1 class="
          text-xs-center 
          text-sm-center 
          text-md-center 
          color-custom">Kenapa #KiosTixAja?</h1>
      </v-flex>
      
      <v-flex 
        offset-md4
        md4>
        <div class="
            text-xs-center 
            text-sm-center 
            text-md-center 
            margin-bottom-1 
            color-custom">
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
      videoId: 'IM-6ZqJURcI'
    }
  },
  components: {
    youtube
  }
}
</script>

<style scoped>
  .section-one{
    background-image: url("https://www.w3schools.com/w3images/photographer.jpg");
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
</style>
