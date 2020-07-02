<template>
  <section class="mt-12">
    <v-container class="mt-sm-6">
      <v-card flat>
        <p class="display-1">
          Lastest Stories
        </p>
        <hr class="red darken-1" />
      </v-card>
      <v-row>
        <v-col cols="12" sm="6" md="4" v-for="item in item" :key="item.title">
          <nuxt-link :to="item.link" style="text-decoration: none">
            <v-card>
              <img
              :src="item.src"
              class="img"
              alt=""
              id="New"
            />
            <div style="width: 100%" :height="item.height">
              <v-container>
                <p class="pt-4 pb-4 black--text text-capitalize" >{{ item.title }}</p>
              </v-container>
            </div>
            </v-card>
          </nuxt-link>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  components:{
  },
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

      {
        title:
          'Apply now! The Japanese standard IT school offers 150% of its 100% sponsorships',
        link: '/resultnews/sponsorship',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1593367523/New2/news11-min_2_y4mplo.jpg',
        height: '220'
      },
    ]
  })
}
</script>

<style lang="scss" scoped>
.img {
  max-width: 100%;
}
</style>
