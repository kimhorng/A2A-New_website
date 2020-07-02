<template>
  <div class="mt-6">
    <section class="mt-12 mb-12">
      <v-container>
        <div class="">
          <p>Sabay NEWS &nbsp; | &nbsp; Wed, 25 Septermber, 2019</p>
          <p class="display-1 text-capitalize" style="margin-top: -15px">
            Great! Just an internship, Cambodian students make a lot of cool programs
          </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
        src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1593364269/New2/news10-min_whbp0n.jpg"
        class="img mx-auto pt-md-12 pb-6"
        alt=""
        id="Img" 
      />
      <v-container>
        <v-row class="mx-auto">
          <v-col md="10" sm="12" class="mx-auto">
            <p>
              Studying the theory in the class not directly applicable is not enough for today's university students. Practicing will help students 
              sharpen the knowledge they have learned and better prepare them for the real job market.
            </p>
            <p>
              In order to sharpen the students to another level of study skills, Kirirom Institute of Technology requires all students to undertake an 
              internship on a project offered by various partners, especially the vKirirom resort.
            </p>
            <p>
              Previous internships at Kirirom Institute of Technology include: VK Club mobile app development, face-to-face system management, face-to-face scanning, 
              accessibility of VR devices, ticketing system, and registration. Many other internships students are conducting directly with the Institute's 
              partner companies.
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
        title: 'One student tells the experience of a Japanese standard school, Fantastic!',
        link: '/resultnews/standardschool',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593366235/New2/new5-min_2_xog0ts.jpg',
        height: '220'
      },

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
