<template>
  <div class="mt-6">
    <section class="mt-12 mb-12">
      <v-container>
        <div class="">
          <p>NORKOR THOM DAILY &nbsp; | &nbsp; Thu, 10 September, 2016</p>
          <p class="display-1 text-capitalize" style="margin-top: -15px">
            Japanese Investor Plans $2 Million To Invest In Cambodia's First Membership Resort
          </p>
        </div>
      </v-container>
    </section>

    <section class="info">
      <img
        src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1593362130/New2/newss7-min_jeel4d.jpg"
        class="img mx-auto pt-md-12 pb-6"
        alt=""
        id="Img" 
      />
      <v-container>
        <v-row class="mx-auto">
          <v-col md="10" sm="12" class="mx-auto">
            <p>
              Japanese investors from Japanese company A2A Town Cambodia will invest about $ 2 million to 
              build a membership resort similar to a hotel or apartment on the top of Kirirom Mountain in 2017.
            </p>
            <p>
                  Takeshi Izuka, president of A2A Town Cambodia, said over the weekend that Membership Resort plans to require members 
                  to register as members to purchase the resort for $ 20,000, which is valid for 45 years. Members can stay on their own, 
                  but if their relative wants to stay, they have to pay $ 30 per night and pay $ 400 per year for building and room maintenance services. 
                  He added that the Membership Resort is a five-star hotel with modern amenities, and it is quiet because the hotel is located on the 
                  highest mountain of Preah Monomom: Kirirom National Park. The sink or beautiful view of the mountain.  <br>                                                                                                                             
                  “You see a lot of rich Cambodians, they don't want to live in crowded places and a diverse group of people, rich and middle-class, 
                  so I invest in Membershipresort,” he said. Come up to meet your needs, leisure and personal services. ” "The concept of this project 
                  is that I want everyone to come here and have fun and make them feel like their second home when they come and stay here," he said.
            </p>
            <p>
                  The MembershipResort project will begin selling later this year and begin construction in early 2017. The project will take one year 
                  to complete and allow members to stay in the initial phase. The first step, each building is three stories high and has a total of 85 
                  square meters that can accommodate four or more people.
            </p>
            <p>
                  Ho Vandy, secretary-general of the National Tourism Association of Cambodia, said it is a new service where members can get a special 
                  price for lodging, but he does not know how many local and foreign clients invest. Such a paid membership service is like buying a 
                  mortgage and can sell the service, he said Any owner may terminate this service. Minister of Tourism Thong Khon said the project was 
                  very good because tourists, when they know it is a green environment protection project, they will not be afraid to spend money because 
                  they They know that they can contribute to environmental protection at their expense, which means they can contribute to environmental protection.
            </p>
            <p>
                  "He supports the project, the project is good because the developer has done a good job of preserving the environment and trying not to touch(cut) the tree."
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
