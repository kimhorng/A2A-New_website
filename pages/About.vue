<template>
  <div id="Hold-About" class="mt-12">
    <v-row class="primary hidden-sm-and-down">
      <v-col
        sm="12"
        md="6"
        cols="12"
        class="about_text hidden-sm-and-down"
        style="height: 700px"
      >
        <v-container style="height: 100%;  width: 90%">
          <p class="display-1" style="position: relative; float: left; top: 50%; left: 50%; transform: translate(-50%, -50%);">
            Creating world-class experiences in Cambodia
          </p>
        </v-container>
      </v-col>
      <v-col sm="12" md="6" cols="12" class="about_image">
      </v-col>
    </v-row>
    <div class="about_image hidden-md-and-up">
      <v-container
          style="height:100% "
          class="primary--text "
        >
          <p
            class="display-1 mobile_text text-center"
            style="position: relative; float: left; top: 50%; left: 50%; transform: translate(-50%, -50%);"
          >
            Creating world-class experiences in Cambodia
          </p>
        </v-container>
    </div>

    <div id="M-Content" style="margin-left: 0px; margin-right:0px ">
      <div class="section" style="margin-left: 0px; margin-right:0px ">
        <v-row class="white py-lg-12 py-md-12" style="margin-left: 0px; margin-right:0px ">
          <v-col lg="6" md="12" sm="12" cols="12" class="mb-lg-12" style="margin-left: 0px; margin-right:0px ">
            <v-container class="headline mt-sm-3" >
              <p class="mx-lg-12 px-lg-12 px-md-12 mx-md-12 mx-sm-12 pt-8 pt-sm-12 font-weight-bold" style="margin-left: 0px; margin-right:0px ">Who Are We?</p>
            </v-container>
          </v-col>

          <v-col lg="6" md="12" sm="12" cols="12">
            <v-container>
              <p
                class="mx-lg-12 px-lg-12 px-md-12 mx-md-12 mx-sm-12 Content"
                id="P"
                style="margin-left: 0px; margin-right:0px "
              >
                We are the team behind the vKirirom Nature Land Project, that
                includes Kirirom Institute of Technology, vKirirom Pine Resort,
                A2A Digital and Property Development
              </p>
            </v-container>
          </v-col>
        </v-row>
      </div>
  </div>
  <section>
    <History />
  </section>
      <div class="py-12 primary">
        <v-card flat class="mx-auto">
          <v-container>
            <v-row class="mx-auto">
              <v-col md="10" sm="12" class="mx-auto">
                <h3 class="mb-3 text-center">
                  More About Us
                </h3>
                <div class="Content ">
                  <v-container>
                    <div>
                      <p class="pt-4"> A2A Town Cambodia is presently working on the main
                      project, “vKirirom” meaning Kirirom is for everyone, of developing
                      Kirirom National Park in Cambodia.
                      </p>
                    </div>
                    <div>
                      <p class="pt-4">Our shareholders are from vKirirom Pte.Ltd. 100% With the
                      increasing and improvement of living standards, A2A will soon
                      become a big market player in the world. We see massive potential
                      in Cambodia and want to create something that is world-class.
                      </p> 
                    </div>
                    <div>
                      <p class="pt-4">In this project, It’s including vKirirom Pine Resort(
                    Glamping and Villas),  Kirirom Institute of Technology (A
                    University which is focusing Technology and Management),
                    Creative Forest (Biggest Auditorium in Asia) and besides from
                    that, we provide IT Services and real estate business
                    as the second home for everyone to come and enjoy with the best
                    experience in our eco-tourism. We believe that vKirirom is
                    the place where people should visit at least once in their lifetime.</p>
                    </div>
                  </v-container>
                </div>
              </v-col>
            </v-row>
          </v-container>
          <v-col class="text-center">
            <v-btn
              flat
              outlined
              width="160"
              class="my-6"
              color="red darken-1"
              to="/executiveboard"
              id="Btn"
            >
              Meet Our Leader
            </v-btn>
          </v-col>
        </v-card>
      </div>
      <div class="section">
        <Carousel />
      </div>
    
    <footer class="white">
      <Footer />
    </footer>
  </div>
</template>

<script>
import Carousel from '../components/About/Carousel'
import History from '../components/About/History'
import Footer from '../layouts/Footer'
export default {
  data: () => ({
    Hide: false
  }),
  components: {
    Carousel,
    History,
    Footer
  }
}
</script>

<style lang="scss" scoped>
#Btn{
  transition: 1s;
}
#Btn:hover{
  margin-left: 10px;
}
#Hold-About {
  background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766627/News/forest-min_eq3lbt_umrhem.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}
.about_image{
  max-width: 100%;
}
@media screen and (max-width: 600px) {
  .about_image {
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766605/A2A%20Image/pvkAbout_hcxijc_hor5dx.jpg');
    background-size: cover;
    height: 400px;
  }
}
@media screen and (min-width: 600px) {
  .about_image {
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766605/A2A%20Image/pvkAbout_hcxijc_hor5dx.jpg');
    background-size: cover;
    height: 700px;
  }
}
@media screen and (min-width: 960px) {
  .about_image {
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766605/A2A%20Image/pvkAbout_hcxijc_hor5dx.jpg');
    background-size: 100%, contain, contain, cover;
    background-position: bottom, 0% 30%, 0% 30%, center;
    height: 700px;
  }
}
</style>
