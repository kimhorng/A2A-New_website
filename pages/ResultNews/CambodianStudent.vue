<template>
  <div class="mt-6">
    <section class=" mb-12 mt-12">
      <v-container>
        <div class="">
          <p>Sabay NEWS &nbsp; | &nbsp; Thu, 03 October, 2019</p>
          <p class="display-1 text-capitalize" style="margin-top: -15px">
            Another excitement! A Cambodian Student tells about learning struggle until reaching the goal to work at Japan
          </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
            src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1593362130/New2/newss6-min_z77ljl.jpg"
            class="img mx-auto pt-md-12 pb-6"
            alt=""
            id="Img" 
      />
      <v-container>
        <v-row class="mx-auto">
          <v-col md="10" sm="12" class="mx-auto">
            <p>
              “Getting a job offer in Japan makes me visualize my dream more precisely with this I also get ready 
              to face any new challenge in order to expand my capacity stronger then when I come back I want to open 
              IT company” this is the delighted description from Ro Vine, the first-generation graduate student Kirirom 
              Institute of Technology.
            </p>
            <p>
              “Studying at KIT, I am trained in both technology skill and communication accompanied by regular 
              practice that can help me work professionally so I am confident that I will be able to get the 
              job done, even in an abroad environment” he added.
            </p>
            <p>
              He shared with the next generation that “ to be able to reach our dream we have to be patient, work-hard, 
              spend the time and do not hesitate as long as we have high commitment, w e will certainly do it”. 
            </p>
            <p>
              “Ro Vine” is one of the outstanding students among many students who got a job offer in Japan after graduation 
              successfully from Kirirom Institute of Technology.
            </p>
            <p>
              In addition to describing the happy story, he also pointed out the difference between dreaming and experiencing 
              reality in the path of study life and work as well.
            </p>
            <p>
              Kirirom Institute of Technology (KIT) is an institute that was established in 2014 by Japanese investor Takeshi 
              Izuka to contribute to human resource development in Cambodia.
            </p>
            <p>
              Especially for the 2019-2020 school year, this standard institute of technology has decided to offer 100% 
              of its scholarships to Cambodian students on skills such as Software Engineering and International Hospitality 
              Management whereas International Hospitality Management, the school is going to open soon. 
            </p>
            <p>
              Besides providing a scholarship of 100% on the cost of a bachelor’s degree, the institute also includes tuition fees, 
              accomodation, meals, transportation, study materials, health care, and other accident insurance. 
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

      {
        title:
          'Apply now! The Japanese standard IT school offers 150% of its 100% sponsorships',
        link: '/resultnews/sponsorship',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593367523/New2/news11-min_2_y4mplo.jpg',
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
