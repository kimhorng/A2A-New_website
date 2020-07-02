<template>
  <div class="mt-6">
    <section class="mt-12 mb-12">
      <v-container>
        <div class="">
          <p>Sabay NEWS &nbsp; | &nbsp; Sun, 15 Septermber, 2019</p>
          <p class="display-1 text-capitalize" style="margin-top: -15px">
            Graduate High School, ready to learn IT? One student tells the experience of a Japanese standard school, Fantastic!
          </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
        src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1593362133/New2/newss5-min_douqpi.jpg"
        class="img mx-auto pt-md-12 pb-6"
        alt=""
        id="Img" 
      />
      <v-container>
        <v-row class="mx-auto">
          <v-col md="10" sm="12" class="mx-auto">
            <p>
              Recently, a student opened up about his experiences beyond expectations during a full-year undergraduate course at Kirirom Institute of Technology (KIT). 
              One posted on the official Facebook page of the Kirirom Institute of Technology.
            </p>
            <p>
              In the video, a first-year student, Sin Sovannmony, made it clear that the whole year they came to school was very enjoyable because there was a better 
              atmosphere to promote learning and taught by foreign teachers full of knowledge, skills and experience, always paying attention to their studies.
            </p>
            <p>
              Not only the scholarships, the IT school also provides Ipad, Computer, clean rooms, bathrooms with both cold and hot water and Wifi.
            </p>
            <p>
              More specifically, Sovannmony also does not have to spend time doing laundry or cooking himself, because all of this school provides the whole thing, 
              which gives him enough time to focus on his studies.
            </p>
          </v-col>
        </v-row>
      </v-container>
    </section>
    <section class="info pb-sm-12 pb-6">
      <v-container>
        <p class="display-1">
          Related Posts
        </p>
        <v-row>
          <v-col cols="12" sm="6" md="4" v-for="item in item" :key="item.title">
            <nuxt-link :to="item.link"  style="text-decoration: none">
              <v-card>
                <img :src="item.src" class="img" alt="" width="100%"/>
                <div style="width: 100%" :height="item.height">
                  <v-container>
                    <p class="pt-4 pb-4 black--text text-tranfrom">{{ item.title }}</p>
                  </v-container>
                </div>
              </v-card>
            </nuxt-link>
          </v-col>
        </v-row>
      </v-container>
    </section>
    <footer>
      <footer2/>
    </footer>
  </div> 
</template>

<script>
import footer2 from '../../layouts/Footer'
export default {
  data: () => ({
    item: [
       
      {
        title:
          'Apply now! The Japanese standard IT school offers 150% of its 100% sponsorships',
        link: '/resultnews/sponsorship',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593367523/New2/news11-min_2_y4mplo.jpg',
        height: '220'
      },
       
      {
        title:
          'Japanese Company To Invest $500 Million To Develop Kirirom National Park',
        link: '/resultnews/japanesecompany',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1591369036/New2/news3-min_v6gtqm.jpg',
        height: '220'
      },
      
      {
        title: 'A $500 Million Retirement Home Project In Kirirom Is Attracting Japanese Tourists',
        link: '/resultnews/Japanesetourists',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1591369329/New2/news2-min_glzbhg.jpg',
        height: '220'
      },
    ]
  }),
  components: {
    footer2
  }
}
</script>

<style lang="scss" scoped>
#Img {
  max-width: 100%;
  display: block;
  margin-left: auto;
  margin-right: auto;
}

</style>
