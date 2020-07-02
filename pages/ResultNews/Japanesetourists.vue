<template>
  <div class="mt-6">
    <section class="mt-12 mb-12">
      <v-container>
        <div class="">
          <p>Sabay NEWS &nbsp; | &nbsp; Fri, 9 June, 2017 14:41</p>
          <p class="display-1" style="margin-top: -15px">
              A $500 Million Retirement Home Project In Kirirom Is Attracting Japanese Tourists To Cambodia </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
        src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1591689007/New2/newss1-min_urxdzb.jpg"
        class="img mx-auto pt-md-12 pb-6"
        alt=""
        id="Img" 
      />
      <v-container>
        <v-row class="mx-auto">
          <v-col md="10" sm="12" class="mx-auto">
            <p>
              The retirement home project, which is in line with the Ministry of Tourism's tourist attraction policy, 
              is officially launched. A Japaneses company have a land concessions totaling 2,000 hectares at the resort 
              of Kirirom, Kampong Speu from the Government of Cambodia to build homes for retired tourists Initially, 
              about $ 500 million was attracting a large number of Japanese tourists to Cambodia. A2A Town Cambodia 
              representative from Japan, Hin Socheat, said the company had been developing a long-term housing project. 
              A simple and luxurious type of accommodation for all types of tourists for both high and low cost travelers, 
              especially tourists retirements.
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

      {
        title:
          "Japanese Investor Plans $2 Million To Invest In Cambodia's First Membership Resort",
        link: '/resultnews/japaneseinvestor',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593362148/New2/new7-min_gtq66n.jpg',
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
