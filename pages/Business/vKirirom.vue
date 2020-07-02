<template>
  <div>
    <div class="hidden-xs-only">
      <section>
        <v-container>
          <v-row wrap class="mt-12 mb-12">
            <v-col cols="12" sm="6" md="6" class="my-auto">
              <h2 id="Title">vKirirom</h2>
            </v-col>

            <v-col cols="12" sm="6" md="6" class="my-auto">
              <p id="Sub" class="mt-5">Make your retreat to the nature</p>
            </v-col>
          </v-row>
        </v-container>
      </section>

      <section>
        <v-row id="Background">
          <v-col class="bg" id="Img" alt="background"></v-col>
        </v-row>
      </section>

      <section style="background-color: #fafafa">
        <v-container>
          <v-row wrap class="mx-auto">
            <v-col cols="10" class="pr-md-12 mx-auto" id="Text">
              <div class="mt-12 mb-12">
                <h2>
                  About vKirirom Pine Resort
                </h2>
                <p class="pt-4">
                  vKirirom Pine Resort is an all-inclusive, eco-resort that
                  offers all kinds of experiences through a vast variety of
                  leisure and educational activities, unique and private
                  lodging, luscious Khmer and international cuisines and the
                  exquisite views of the divine nature of Kirirom National Park,
                  the biggest pine forest in Cambodia.
                </p>
                <p class="pt-4">
                  The weather and natural beauty of Kirirom create a perfect
                  environment for entrepreneurs, residents, and students seeking
                  a living and working space for creativity, health, and
                  innovation. Our duty is to develop ecotourism by making it
                  accessible to all kinds of visitors while protecting its
                  beauty for many generations to come through eco-friendly
                  sustainable development.
                </p>
                <p class="pt-4">
                  The weather and natural beauty of Kirirom create a perfect
                  environment for entrepreneurs, residents, and students seeking
                  a living and working space for creativity, health, and
                  innovation.
                </p>
                <p class="pt-4">
                  Our resort is perfect for off-the-beaten-path family
                  vacations, educational field trips, annual company retreats,
                  business travels, and organizing special events.
                </p>

                <h2 class="pt-4">Accommodations</h2>
                <ul class="pt-4">
                  <li>Bell Tent</li>
                  <li>Bungalow</li>
                  <li>Luxury Tent</li>
                  <li>Piperoom</li>
                  <li>Khmer Cottage</li>
                  <li>Villa Suite</li>
                  <li>Villa Jasmine</li>
                  <li>Solo Camping</li>
                  <li>Couple Camping</li>
                  <li>Family camping</li>
                </ul>

                <h2 class="mt-4 pt-4">Menu</h2>
                <ul class="pt-4">
                  <li>Healthy</li>
                  <li>Khmer</li>
                  <li>Western</li>
                  <li>Chinese and Thai</li>
                  <li>Indian</li>
                  <li>Japanese</li>
                  <li>Desserts</li>
                </ul>
              </div>
            </v-col>
          </v-row>
        </v-container>
      </section>

      <section class="each_link">
        <v-row style="height: 100%">
          <v-flex class="my-auto">
            <div class="text-center">
              <a href="https://vkirirom.com/" target="_blank" id="btn" style="text-decoration:none">
                <v-btn width="180px" primary light outlined class="mx-auto secondary1--text text-capitalize">
                  <span class="title">Book a Retreat</span>
                </v-btn>
              </a>
            </div>
          </v-flex>
        </v-row>
      </section>

      <section class="info pt-4">
        <v-container>
          <div class="text-center">
            <p> For more information,</p>
            <p>Visit our Facebook page: <a href="https://web.facebook.com/vkirirom/" target="_blanck" style="color: black">vKirirom Pine Resort</a></p> 
            <p>Send us an email: info@vkirirom.com</p> 
            <p>Call: +855 (0)78 777 284</p>
          </div>  
        </v-container>  
      </section>      

      <section class="footer">
        <div class="img_responsive">
          <nuxt-link to="/business/a2adigital" class="link">
            <div class="last_img">
              <v-row class="blur">
                <v-flex class="my-auto">
                  <div class="text-center">
                    <p  class="display-1">Next Project</p>
                  </div>
                </v-flex>
              </v-row>
            </div>
          </nuxt-link>
        </div>
      </section>
    </div>

    <div class="hidden-sm-and-up">
      <v-carousel
        :continuous="false"
        :show-arrows="false"
        hide-delimiter-background
        delimiter-icon="mdi-minus"
        height="100%"
      >
        <v-carousel-item>
          <vkirirom />
        </v-carousel-item>

        <v-carousel-item>
          <a2aDigital />
        </v-carousel-item>

        <v-carousel-item>
          <kit />
        </v-carousel-item>

        <v-carousel-item>
          <property />
        </v-carousel-item>
      </v-carousel>
    </div>
    <footer>
      <Footer/>
    </footer> 
  </div>
</template>
<script>
import a2aDigital from '../business1/a2aDigital'
import kit from '../business1/kit'
import property from '../business1/property'
import vkirirom from '../business1/vKirirom'
import Footer from '../../layouts/Footer'
export default {
  components: {
    a2aDigital,
    kit,
    property,
    vkirirom,
    Footer
  }
}
</script>
<style scoped>
#btn{
  transition: 1s;
}
#btn:hover{
  margin-left: 10px;
}
h2 {
  margin-top: 3px;
  margin-bottom: 6px;
}
h3 {
  margin-bottom: 12px;
}
.img-responsive {
  max-width: 100%;
}
.link {
  text-decoration: none;
}
@media screen and (max-width: 960px) {
  .all_text {
    height: 1400px;
  }
  .each_link {
    height: 400px;
  }
  .footer {
    height: 400px;
  }
  .last_img {
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766597/A2A%20Image/a2a_digital-min_l568ad_uircnc.jpg');
    background-size: 100%, 100%, 100%, cover;
    max-width: 100%;
    height: 400px;
  }
  .blur {
    height: 400px;
    background-color: black;
    opacity: 0.5;
  }
  .bg {
    height: 500px;
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591939083/Homepage/vkirirom_res_1_mwjolw.jpg');
    background-size: 100%, 100%, 100%, cover;
  }
}
@media screen and (min-width: 960px) {
  .each_link {
    height: 700px;
  }
  .footer {
    height: 700px;
  }
  .last_img {
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766597/A2A%20Image/a2a_digital-min_l568ad_uircnc.jpg');
    background-size: 100%, 100%, 100%, cover;
    max-width: 100%;
    height: 700px;
  }
  .blur {
    height: 700px;
    background-color: black;
    opacity: 0.5;
  }
  .bg {
    height: 800px;
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591939083/Homepage/vkirirom_res_1_mwjolw.jpg');
    background-size: 100%, 100%, 100%, cover;
  }
}
</style>
