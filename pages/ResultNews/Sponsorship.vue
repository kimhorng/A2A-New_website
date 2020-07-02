<template>
  <div class="mt-6">
    <section class="mt-12 mb-12">
      <v-container>
        <div class="">
          <p> BUSINESS CAMBODIA &nbsp; | &nbsp; 30 May, 2019</p>
          <p class="display-1 text-capitalize" style="margin-top: -15px">
            Apply now! The Japanese standard IT school in Kirirom offers 150% of its 100% scholarships          
          </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
        src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1593366488/New2/newss11_v3d2na.jpg"
        class="img mx-auto pt-md-12 pb-6"
        alt=""
        id="Img" 
      />
      <v-container>
         <v-row class="mx-auto">
           <v-col md="10" sm="12" class="mx-auto">
             <p>
              Recently, according to the Facebook page of the Kirirom Institute of Technology, as well as the official website of the Ministry of Education, 
              Youth and Sport, the institute has provided 100% scholarships to approximately 150 students. For those who wish to attend the 2019-2020 school year.
            </p>
            <p>
              According to the application form provided to students, Kirirom Institute of Technology offers two scholarships: Software Engineering and International Hospitality Management.
            </p>
            <p>
              Those who are interested in taking the scholarship exam can go to the registry link: https://goo.gl/forms/ly8zdI6Q18jaqqg03. After registration, 
              candidates will be able to visit the Directory Seminar organized by the institute in person while the exam will be held on the 29th of June. 2019 at the Japan-Cambodia Cooperation Center.
            </p>
            <p>
              Kirirom Institute of Technology has been established since 2014 with programs such as Computer Engineer, Computer System Analysis, Develop a Computer System, Accounting and Management as 
              well as teaching English and Japanese. 
            </p>
            <p>
              The institute, located in the national park of nature, was founded by a Japanese man named Takeshi Izuka to provide high quality education to Cambodian students; especially in 
              computer science and software engineering.
            </p>
            <p>
              As a result of the institute's training, first-generation students are given 100% job opportunities, and up to 70% of students went to work in Japan.
            </p>
            <p>
              In order to qualify, candidates must be at least 16 years of age and have a high school diploma to obtain a scholarship. The exam is administered in IQ, Maths and English, and candidates must 
              pass an interview.
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

      {
        title:
          ' Kirirom Will Be A Natural City While A Japanese Company Vows To Develop',
        link: '/resultnews/naturalcity',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1591369199/New2/news1-min_bauwlr.jpg',
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
