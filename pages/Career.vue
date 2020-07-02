<template>
  <div class="mt-12">
    <section class="mt-sm-6">
      <v-container>
        <v-row wrap class="text">
          <v-col cols="12">
            <h1 align="center" class="display-1" id="Title">
              Join our team make an impact
            </h1>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <section>
      <v-row class="mt-6 mx-auto">
        <iframe
          id="Img"
          width="95%"
          height="700px"
          class="img-responsive mx-auto"
          src="https://www.youtube.com/embed/P0Napv0lrI8"
          frameborder="0"
          allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        >
        </iframe>
      </v-row>
    </section>

    <section>
      <v-container>
        <v-row>
          <v-col cols="12" sm="10" class="mx-auto">
            <p class="headline font-weight-bold">We're hiring!</p>
          </v-col>
        </v-row>

        <v-row v-for="career in careers" :key="career.title">
          <v-container>
            <v-col
              md="10" sm="12"
              class="pr-md-0 pl-md-0 mx-auto"
              style="padding-right: 12px;padding-left: 12px;"
            >
              <v-card >
                <nuxt-link :to="career.link">
                  <v-container>
                  <h2 class="secondary1--text">
                    {{ career.title }}
                  </h2>
                  <p class="black--text">{{ career.working_hour }}</p>
                </v-container>
                </nuxt-link>
              </v-card>
            </v-col>
          </v-container>
        </v-row>
      </v-container>
    </section>
    <v-card
      class="grey lighten-5 text-center pt-12 mt-12"
      flat
      height="200"
    >
      <p class="grey--text">Contact us</p>
      <div class="display-1">recruit@asiato.asia</div>
    </v-card>

    <!--  -->
    <v-card flat class="text-center py-12  mt-3">
      <v-img
        src="https://cuberto.com//assets/img/contacts/alexandria.png"
        width="100"
        class="mx-auto"
        alt="House"
      />
      <p id="Title">Phnom Penh</p>
      <p class="grey--text">vKirirom Head Office, Borey Chouk Meas</p>
      +855 12 345 678
    </v-card>
    <footer>
      <Footer/>
    </footer> 
  </div>
</template>

<script>
import Footer from '../layouts/Footer'
export default {
  components:{
    Footer
  },
  data: () => ({
    careers: [
      {
        title: 'Facilities Manager',
        working_hour: 'FULL-TIME, KIRIROM INSTITUTE OF TECHNOLOGY',
        link: '/jobinfo/hospitalitylecturer'
      },
      {
        title: 'Hospitality and Tourism Lecturer',
        working_hour: 'FULL-TIME, KIRIROM INSTITUTE OF TECHNOLOGY',
        link: '/jobinfo/hospitalitylecturer'
      },
      {
        title: 'Math Lecturer',
        working_hour: 'FULL-TIME, KIRIROM INSTITUTE OF TECHNOLOGY',
        link: '/jobinfo/mathlecture'
      },
      {
        title: 'Student Counsellor',
        working_hour: 'FULL-TIME, KIRIROM INSTITUTE OF TECHNOLOGY',
        link: '/jobinfo/studentcounsellor'
      },
      {
        title: 'HR and Admin Officer',
        working_hour: 'FULL-TIME, KIRIROM INSTITUTE OF TECHNOLOGY',
        link: '/jobinfo/admin'
      },
      {
        title: 'Accounting Lecturer',
        working_hour: 'PART-TIME, KIRIROM INSTITUTE OF TECHNOLOGY',
        link: 'jobinfo/accountinglecturer'
      },
      {
        title: 'Khmer Culture and History Lecturer',
        working_hour: 'FULL-TIME, KIRIROM INSTITUTE OF TECHNOLOGY',
        link: 'jobinfo/historylecturer'
      },
      {
        title: 'IT Lecturer',
        working_hour: 'FULL-TIME, KIRIROM INSTITUTE OF TECHNOLOGY',
        link: 'jobinfo/ITlecturer'
      },
      {
        title: 'Head of Department of Tourism Management',
        working_hour: 'FULL-TIME, KIRIROM INSTITUTE OF TECHNOLOGY',
        link: 'jobinfo/tourismmanagement'
      }
    ]
  })
}
</script>

<style lang="scss" scoped>
.img-responsive {
  max-width: 100%;
}
</style>
