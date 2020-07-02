<template>
  <div class="">
    <section class="mt-12 mb-12">
      <v-container>
        <div class="">
          <p class="pt-sm-6">Reksmey Kampuchea &nbsp; | &nbsp; September 11, 2019, 3:11 PM</p>
          <p class="display-1" style="margin-top: -15px">
            KIT Institute Welcome The Students Who Passed The International Exam
          </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
        src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1591689007/New2/newss2-min_xw3mur.jpg"
        class="img pt-md-12 pb-6"
        alt=""
        id="Img"
      />
      <v-container>
        <v-row class="mx-auto">
          <v-col md="10" sm="12" class="mx-auto">
            <p>
              Students who have completed high school diploma or passed international exam can choose a sponsorship at the Kirirom 
              Institute of Technology (KIT) with free four years, including study materials.
            </p>
            <p>
              According to the Facebook page of the Kirirom Institute of Technology as well as the official page of the 
              Ministry of Education, Youth and Sport of the Kingdom of Cambodia, said last week that the sponsorship 
              will be offered to graduates of the 12th grade in the 2019-2020 school year. The institute has launched a 
              new sponsorship program for Cambodian students completing their high school diploma in the 2019-2020 school year. 
              The test will receive a 100 percent sponsorship plus four years of study materials.
            </p>
            <p>
              Kirirom Institute of Technology offers two sponsorships: Software Engineering and secondly International Hospitality Management.
            </p>
            <p>
              Students who wish to take the sponsorship exam can go to the following link: https: //goo.gl/forms/ly8zdI6Q18jaqqg03. After registration, 
              candidates will be able to join the introductory orientation that is hosted by the institute and exam day will be held on 29th of June, 
              2019 at the Cambodia-Japan Cooperation Center.
            </p>
            <p>
              Kirirom Institute of Technology has been established since 2014 with programs such as Computer Engineering, Computer System Analysis, 
              Develop a computer system, Accounting and Management, including teaching English and Japanese. The institute located in Kirirom 
              National Park was established by A2A Town Cambodia CEO Mr. Takeshi Izuka to provide high quality education to Cambodian students, 
              especially in subjects related to computer science and software engineering etc. As a result of the institute's training, 
              first-generation students get 100% job opportunities and up to 70% students went to work in Japan.
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

      {
        title:
          'A Cambodian Student tells about learning struggle Until Reaching The Goal',
        link: '/resultnews/cambodianstudent',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593361816/New2/new6-min_xbhvbd.jpg',
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
