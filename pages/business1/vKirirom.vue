<template>
  <div class="mt-12">
    <section>
      <v-container>
        <v-row wrap class="mx-auto">
          <v-col cols="12" xs="12" sm="12" md="6">
            <h2 id="Title">vKirirom</h2>
          </v-col>

          <v-col cols="12" xs="12" sm="12" md="6">
            <p id="Sub" style="margin-top: -15px">Make your retreat to the nature</p>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <section>
      <v-row id="Background">
        <v-col class="bg" id="Img" alt="background"> </v-col>
      </v-row>
    </section>

    <section>
      <v-row wrap class="mx-auto">
        <v-col cols="12" class="pr-md-12 mx-auto info" id="Text">
          <div class="mt-12 mb-12">
            <v-container>
              <h2>
                About vKirirom Pine Resort
              </h2>
              <p class="pt-4">
                vKirirom Pine Resort is an all-inclusive, eco-resort that offers
                all kinds of experiences through a vast variety of leisure and
                educational activities, unique and private lodging, luscious
                Khmer and international cuisines and the exquisite views of the
                divine nature of Kirirom National Park, the biggest pine forest
                in Cambodia.
              </p>
              <p class="pt-4">
                The weather and natural beauty of Kirirom create a perfect
                environment for entrepreneurs, residents, and students seeking a
                living and working space for creativity, health, and innovation.
                Our duty is to develop ecotourism by making it accessible to all
                kinds of visitors while protecting its beauty for many
                generations to come through eco-friendly sustainable
                development.
              </p>
              <p class="pt-4">
                The weather and natural beauty of Kirirom create a perfect
                environment for entrepreneurs, residents, and students seeking a
                living and working space for creativity, health, and innovation.
              </p>
              <p class="pt-4">
                Our resort is perfect for off-the-beaten-path family vacations,
                educational field trips, annual company retreats, business
                travels, and organizing special events.
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
            </v-container>
          </div>
        </v-col>
      </v-row>
    </section>
    <section>
      <div class="text-center nextProject ">
        <a href="https://vkirirom.com/" target="_blank" id="btn" style="text-decoration:none">
                <v-btn width="180px" primary light outlined class="mx-auto secondary1--text text-capitalize">
                  <span class="title">Book a Retreat</span>
                </v-btn>
        </a>
      </div>
      
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

      <div>
        <nuxt-link to="/business/a2adigital" class="link">
          <div class="last_img" style="height: 350px">
            <div class="text" style="width:100% ; height: 100%">
              <p class="headline">Next Project</p>
            </div>
          </div>
        </nuxt-link>
      </div>
    </section>
  </div>
</template>

<style scoped>
#btn{
  transition: 1s;
}
#btn:hover{
  margin-left: 10px;
}
.img-responsive {
  max-width: 100%;
}
.nextProject {
  margin-top: 150px;
  margin-bottom: 150px;
  max-width: 100%;
}
.nextProPic {
  max-width: 100%;
  opacity: 0.5;
}
.last_img {
  background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766606/A2A%20Image/a2a_digital-min_yhmwll_gueaod.jpg');
  background-size: cover;
}
.link {
  text-decoration: none;
}
.text {
  padding-top: 170px;
  text-align: center;
  background-color: black;
  opacity: 0.5;
}
.bg {
  background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591939472/Homepage/vkirirom_res_1_mto5no.jpg');
  background-size: cover;
  height: 400px;
}
</style>
