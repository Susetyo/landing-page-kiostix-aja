<template>
  <v-layout
    class="
    section-two
    text"
    wrap
    row>
      
 
      <v-flex lg6>
        
        <h1 class="
          text-xs-center 
          text-sm-center 
          text-md-center 
          margin-bottom-1 ">#KiosTixAja!</h1>
 
        <div class="
            text-xs-center 
            text-sm-center 
            text-md-center 
            margin-bottom-1 ">
          Mulai dari pentas seni dan kreasi, tuournament olahraga seminar hingga festival musik, KiosTix siap
          mendapingi event kamu dari awal hingga akhir untuk menghadirkan pengalaman event terbaik.
        </div>
      </v-flex>
      
      <v-flex lg6>
        <v-card>
          <v-container
            fluid
            grid-list-md
          >
            <v-layout row wrap>
              <v-flex
                v-for="card in cards"
                :key="card.title"
                v-bind="{ [`xs${card.flex}`]: true }"
              >
                <v-card>
                  <v-img
                    :src="card.src"
                    height="400px"
                  >
                    <v-container
                      fill-height
                      fluid
                      pa-2
                    >
                      <v-layout fill-height>
                        <v-flex xs12 align-end flexbox>
                          <span class="headline white--text" v-text="card.title"></span>
                        </v-flex>
                      </v-layout>
                    </v-container>
                  </v-img>

                  <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn icon>
                      <v-icon>favorite</v-icon>
                    </v-btn>
                    <v-btn icon>
                      <v-icon>bookmark</v-icon>
                    </v-btn>
                    <v-btn icon>
                      <v-icon>share</v-icon>
                    </v-btn>
                  </v-card-actions>
                </v-card>
              </v-flex>
            </v-layout>
            
          </v-container>
        </v-card>
        
      </v-flex>


  
  
  
  </v-layout>
</template>

<script>
import youtube from '~/components/Youtube.vue';

export default {
  data(){
    return{
       cards: [
        { title: 'Favorite road trips', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 6 },
        { title: 'Best airlines', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 6 }
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
    margin-top: 5rem;
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
</style>
