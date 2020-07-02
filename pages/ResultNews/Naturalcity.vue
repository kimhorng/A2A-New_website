<template>
  <div class="mt-6">
    <section class="mt-12 mb-12">
      <v-container>
        <div>
          <p>Khmerload &nbsp; | &nbsp; 12:03 April 08, 2019</p>
          <p class="display-1 " style="margin-top: -15px">
            Kirirom Will Be A Natural City While A Japanese Company Vows To Develop
        </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
        src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1591689007/New2/newss3-min_hgdlv4.jpg"
        class="img pt-md-12 pb-6"
        alt=""
        id="Img"
      />
      <v-container>
        <v-row class="mx-auto">
          <v-col md="10" sm="12" class="mx-auto">
            <p>
                A2A Town (Cambodia) Co., Ltd. has invested US $ 521 million with a Cambodian partner to develop the 
                Preah Vihear Preah Vihear Preah Kossom-Kushom National Park, an eclectic and culturally rich pine and valleys. 
                The waterfall of the stream creates a natural music atmosphere that the visitors enjoy.          
            </p>
            <p>
              Mr. Takeshi Izuka, Director of A2A Town (Cambodia) Co., Ltd, has invested in transforming Preah Vihear-Kusom 
              National Park and into the Kirirom Eco-Tourism and Institute of Technology (KIT) to provide Cambodians with 
              knowledge and Real expertise, especially information technology and sustainable conservation of natural 
              resources in the region to promote development Green environment and smokeless (tourism) industry in the country. 
              Minister of Commerce HE Pan Soysak urged Japanese investors to work with the Directorate of Trade Promotion to promote 
              the Kirirom Nature City, surrounded by eco-tourism, green technology, and leisure tourism to attract tourists and transform a project. 
              This is a model of development Nature of the countries in the region. Mr. Takeshi Izuka expressed his thanks to Minister Pan Soysak for 
              his support for the Kirirom Nature City project and informed the vision of A2A Town (Cambodia) Co., Ltd to transform the city into a more modern, 
              sustainable way by bringing electric vehicles with new technologies for Japanese and Japanese students studying at KIT to participate in 
              Industry 4.0 and meet current technology market needs. <br>
              It is worth noting that the company currently offers full scholarships to over 200 Cambodian students and provides jobs for over 450 local people.
            </p>
          </v-col>
        </v-row>
      </v-container>
    </section>
    <section class="info pb-sm-12 pb-6">
      <v-container>
        <p class="display-1 mt-6">
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
      
      {
        title: 'Kirirom’s eco-friendly city receives boost from shares',
        link: '/resultnews/ecofriend',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593368084/New2/news-min_kehscx.jpg',
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
  // width: 50%;
}
</style>
