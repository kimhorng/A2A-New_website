<template>
  <div class="mt-6">
    <section class="mt-12 mb-12">
      <v-container>
        <div class="">
          <p>Post News &nbsp; | &nbsp; Wed, June 10, 2017</p>
          <p class="display-1" style="margin-top: -15px">
            Japanese Company to Invest $500 Million To Develop Kirirom National Park
        </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
        src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1591689007/New2/newss4-min_dwvhtd.jpg"
        class="img pt-md-12 pb-6 "
        alt=""
        id="Img"
      />
      <v-container>
        <v-row class="mx-auto">
          <v-col md="10" sm="12" class="mx-auto">
            <p>
              Recently, Takeshi Izuka,resident of Vkirirum Resort, met with Minister of Commerce Pan Soksak and expressed his desire to turn the area into a tourist attraction.
            </p>
            <p>
              Hin Socheat, managing director at WikiLeaks, told Post News Media that the company plans to invest more than US $ 500 million in a 200-hectare luxury resort in Wirairiri Resort.
            </p>
            <p>
              He added that for the project, the villa is v-rowided into three types: Jasmine, Orchid and V.
            </p>
            <p>
              In response, Pan Soksak supported the project and asked the company to develop a master plan on environmental conservation and wildlife conservation in accordance with the standards.
            </p>
            <p>
              It is worth noting that the project is located in Kampong Speu province and is about 140 km from Phnom Penh.
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
                    <p class="pt-4 pb-4 black--text" >{{ item.title }}</p>
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
        title: 'A $500 Million Retirement Home Project In Kirirom Is Attracting Japanese Tourists',
        link: '/resultnews/Japanesetourists',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1591369329/New2/news2-min_glzbhg.jpg',
        height: '220'
      },

      {
        title:
          ' Kirirom Will Be A Natural City While A Japanese Company Vows To Develop',
        link: '/resultnews/naturalcity',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1591369199/New2/news1-min_bauwlr.jpg',
        height: '220'
      },
      
      {
        title: 'KIT Institute Welcome The Students Who Passed The International Exam',
        link: '/resultnews/kit',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1591369038/New2/news4-min_sxihgz.jpg',
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
  // margin-top: 2.5%;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
