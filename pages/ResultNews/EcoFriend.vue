<template>
  <div class="mt-6">
    <section class="mt-12 mb-12">
      <v-container>
        <div class="">
          <p>KHMER TIMES &nbsp; | &nbsp;  17 October, 2017</p>
          <p class="display-1 text-capitalize" style="margin-top: -15px">
            Kirirom’s eco-friendly city receives boost from shares
          </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
        src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1593362672/New2/newss8-min_rjaiaz.jpg"
        class="img mx-auto pt-md-12 pb-6"
        alt=""
        id="Img" 
      />
      <v-container>
        
          <v-row class="mx-auto">
            <v-col md="10" sm="12" class="mx-auto">
              <p>
                vKirirom, the Japanese holding company in charge of vKirirom Nature City, has succeeded in collecting $5.3 million through 
                third-party allocation of new shares, according to a recent article published in the Japan Times.
              </p>
              <p>
                    vKirirom, the Japanese holding company in charge of vKirirom Nature City, has succeeded in collecting $5.3 million 
                    through third-party allocation of new shares, according to a recent article published in the Japan Times. vKirirom 
                    also holds A2A Town Cambodia, the entity behind the vKirirom Pine Resort and the Kirirom Institute of Technology (KIT).
              </p>
              <p>
                  Takeshi Izuka, president of A2A Town Cambodia, said vKirirom Nature City aims to take advantage of the world’s latest 
                  IT trends to create a sustainable city with an IT university at its core.
              </p>
              <p>
                    “We aim for higher growth by providing greater amounts of educational institutions and opportunities, better living 
                    environments, developing leisure facilities and working places to non-Cambodian investors, starting from those coming from Japan,” Mr Izuka said.
              </p>
              <p>         
                    “We will also be strengthening our operation structure and marketing scheme for further business expansions.”
              </p>
              <p>
                    vKirirom Nature City is home to the Kirirom Institute of Technology (KIT), an academic institution with a world-class IT engineering training program. 
                    According to the Japanese company, programs like this are needed to put an end to Japan’s loss in competitiveness due to a shortage of IT engineers.
              </p>
              <p>
                    “We seek a solution to the accelerating aging population and educational gap through internet and AI-based education systems, innovation in tourism using 
                    shared economy and pursuit of AI innovation in urban and industrial standards, as well as modern living.”
              </p>
              <p>
                    Built over 10,000 hectares of land inside Kirirom National Park, vKirirom Nature City is an urban development project that seeks to integrate eco-tourism principles.
              </p>
              <p>
                    “This project currently consists of KIT, vKirirom Pine Resort and vKirirom Second Home, which conducts the planning, constructing and contracting of sub-leases for the 
                    dormitories. We are constantly seeking to develop this business and increase the vKirirom community,” Mr Izuka added.
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
          'A Cambodian Student tells about learning struggle Until Reaching The Goal',
        link: '/resultnews/cambodianstudent',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593361816/New2/new6-min_xbhvbd.jpg',
        height: '220'
      },

      {
        title:
          'Great! Just an internship, Cambodian students make a lot of cool programs',
        link: '/resultnews/internship',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593366177/New2/news9-min_3_vvkvpl.jpg',
        height: '220'
      },
      
      {
        title: 'One student tells the experience of a Japanese standard school, Fantastic!',
        link: '/resultnews/standardschool',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593366235/New2/new5-min_2_xog0ts.jpg',
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
