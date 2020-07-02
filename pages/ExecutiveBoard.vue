<template>
  <div>
    <section>
      <v-container>
        <v-row class="mt-12">
          <v-flex>
            <h4 class="text-center display-1 mb-12 mt-12 ">
              Meet our leadership team
            </h4>
          </v-flex>
        </v-row>

        <!-- The left size of managers' photo -->

        <div v-for="item in item1" :key="item.name1">
          <v-row wrap class="mt-sm-12">
            <v-col cols="12" md="6" sm="6" class="pic1">
              <v-card flat>
                <img :src="item.img1" class="img-responsive" alt="our-leader" />
              </v-card>
            </v-col>
            <v-col cols="12" md="6" sm="6" class="section1">
              <div class="management1 ">
                <hr
                  class="hidden-xs-only secondary1"
                  style="width: 50% ;border: 1.2px solid #E53935;"
                />
                <div
                  class="pt-6 pb-6"
                  style="width: 80%; margin-left: auto; margin-right: auto"
                >
                  <h3>{{ item.name1 }}</h3>

                  <p class="mt-6">{{ item.position1 }}</p>

                  <v-container>
                    <v-row>
                      <v-card
                        flat
                        v-if="item.btn1 == !btn1"
                        class="secondary1--text"
                        @click="item.btn1 = !item.btn1"
                        id="icon"
                      >
                        View more
                        <v-icon v-if="item.btn1 == true" color="secondary1">
                          mdi-chevron-down
                        </v-icon>
                      </v-card>
                    </v-row>
                  </v-container>
                </div>

                <!-- will show after clicking view more -->

                <div
                  v-if="item.btn1 == false"
                  class="pb-6"
                  style="width: 80%; margin-left: auto; margin-right: auto ;"
                >
                  <hr class="mb-6" />
                  <p>{{ item.background }}</p>

                  <v-container>
                    <v-row>
                      <v-card
                        flat
                        color="secondary1--text"
                        @click="item.btn1 = !item.btn1"
                        id="icon"
                      >
                        View Less
                        <v-icon color="secondary1">
                          mdi-chevron-up
                        </v-icon>
                      </v-card>
                    </v-row>
                  </v-container>
                </div>
              </div>
            </v-col>
          </v-row>

          <!-- The right size of the managers's photo -->

          <v-row wrap class="mt-12">
            <v-col cols="12" md="6" class="hidden-sm-and-up pic2">
              <v-card flat>
                <img :src="item.img2" class="img-responsive" alt="leader" />
              </v-card>
            </v-col>

            <v-col cols="12" md="6" sm="6" class="section2 text-end">
              <div class="management2">
                <hr
                  class="hidden-xs-only secondary1  border-top"
                  style="width: 50% ;border: 1.2px solid #E53935;"
                />
                <div class="pt-6 pb-6 mx-auto" style="width: 80% ;">
                  <div class="text-sm-right">
                    <h3>{{ item.name2 }}</h3>

                    <p class="mt-6">{{ item.position2 }}</p>
                  </div>

                  <v-container>
                    <v-row justify-sm="end">
                      <v-card
                        flat
                        v-show="item.btn2 == !btn2"
                        style="color: #E53935"
                        @click="item.btn2 = !item.btn2"
                        id="icon"
                      >
                        View more
                        <v-icon color="#E53935">
                          mdi-chevron-down
                        </v-icon>
                      </v-card>
                    </v-row>
                  </v-container>
                </div>
                <div
                  v-show="item.btn2 == false"
                  class="pb-6 "
                  style="width: 80%; margin-left: auto; margin-right: auto"
                >
                  <hr class="mb-6" />
                  <p class="text-sm-right">
                    {{ item.background2 }} <br />
                    <br />
                    {{ item.P1 }}<br />
                    <br />
                    {{ item.P2 }}
                  </p>

                  <v-container>
                    <v-row justify-sm="end">
                      <v-card
                        flat
                        style="color: #E53935"
                        id="icon"
                        @click="item.btn2 = !item.btn2"
                      >
                        View Less
                        <v-icon color="#E53935">
                          mdi-chevron-up
                        </v-icon>
                      </v-card>
                    </v-row>
                  </v-container>
                </div>
              </div>
            </v-col>

            <v-col cols="12" md="6" sm="6" class="hidden-xs-only">
              <v-card flat>
                <img :src="item.img2" class="img-responsive" alt="leader" />
              </v-card>
            </v-col>
          </v-row>
        </div>

        <div v-for="item in item2" :key="item.name1">
          <v-row wrap class="mt-sm-12">
            <v-col cols="12" md="6" sm="6" class="pic1">
              <v-card flat>
                <img :src="item.img1" class="img-responsive" alt="leader" />
              </v-card>
            </v-col>
            <v-col cols="12" md="6" sm="6" class="section1">
              <div class="management1 ">
                <hr
                  class="hidden-xs-only secondary1"
                  style="width: 50% ;border: 1.2px solid #E53935;"
                />
                <div
                  class="pt-6 pb-6"
                  style="width: 80%; margin-left: auto; margin-right: auto"
                >
                  <h3>{{ item.name1 }}</h3>

                  <p class="mt-6">{{ item.position1 }}</p>

                  <v-container>
                    <v-row>
                      <v-card
                        flat
                        v-if="item.btn1 == !btn1"
                        class="secondary1--text"
                        @click="item.btn1 = !item.btn1"
                        id="icon"
                      >
                        View more
                        <v-icon v-if="item.btn1 == true" color="secondary1">
                          mdi-chevron-down
                        </v-icon>
                      </v-card>
                    </v-row>
                  </v-container>
                </div>
              </div>
            </v-col>
          </v-row>
        </div>
      </v-container>
    </section>
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
  data() {
    return {
      item1: [
        {
          name1: 'Takeshi Izuka',
          position1: 'Founder & Chief Executive Officer of A2A Town Cambodia',
          background:
            'Mr. Takeshi graduated from a department of Science and Engineering at Waseda University, and received a  degree of Master from Tokyo Institute of Technology.He established Digital Forest Inc. in 1998 while working at Andersen Consulting (Accenture now).  With the successful leading of WEB Analytics Company in Japan, the Digital Forest Inc was sold to NTT Communications in 2009. He then was able to set up a business as a second foundation in Singapore in April 2010 due to his strong efforts.',
          btn1: true,
          img1:
            'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766599/A2A%20Image/Takeshi-min_m0j3pk_jmhblv.jpg',

          name2: 'Dr. Phirom Leng',
          position2: 'President of KIT',
          background2:
            'Dr. Phirom Leng finished his BBA in Management at National University of Management, Cambodia in 2003, BEd in Teaching English as a Foriegn Language at Institute of Foreign Languages in his home country in 2005, and Ma in Southeast Asian Studies from Ohio University in 2010. Later on, he went to pursue his PhD in Higher Education at University of Toronto in 2015.',

          btn2: true,
          P1:
            'He has years of experience working in the educational sector as professor, lecturer, teaching assistant and higher education consultant, and research and development.',
          img2:
            'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766583/A2A%20Image/Dr_Phirom-min_dvdzmd_wr4bdd.jpg'
        },
        {
          name1: 'Hicki Okamoto',
          position1: 'Kirirom Pte. Ltd. Director Vice President of Business',
          background:
            'Born in Osaka in 1971, after graduating from the University of Pennsylvania in the United States, he worked as a consultant and business development manager at Accenture and SoftBank, served as a strategist at Microsoft Seattle and a leadership role in global sales. He joined A2A Town Cambodia in 2018 and is responsible for the Resort Division and Business Development Division.',
          btn1: true,
          img1:
            'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766585/A2A%20Image/hicki-min_hrcf7u_g6jbe3.jpg',
          name2: 'Van Sovanny',
          position2: 'A2A Phnom Penh office, Director ',
          background2:
            'Mrs. Vanny finished her Bachelor’s Degree in Management Information System and pursued her Master’s Degree in Management in 2012. She’s received several awards such as Social Contribution to HIV/AIDS Award by World Vision Organization and Outstanding Management Award by A2A Town (Cambodia) Co., Ltd. She acquires a mastery in communication and interpersonal skills, effective leadership, problem solving and team building.',
          btn1: true,
          btn2: true,
          img2:
            'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766600/A2A%20Image/vanny-min_is7oqp_fmrnpc.jpg'
        }
      ]
    }
  }
}
</script>

<style scoped>
.img-responsive {
  width: 100%;
}
#icon:hover {
  font-size: 17.5px;
}
@media screen and (max-width: 600px) {
  .management1 {
    border: 2px solid #e53935;
    width: 95%;
    margin-left: auto;
    margin-right: auto;
  }
  .management2 {
    border: 2px solid #e53935;
    width: 95%;
    margin-left: auto;
    margin-right: auto;
  }
  .section1 {
    margin-top: -10%;
    z-index: 2;
  }
  .section2 {
    margin-top: -10%;
    z-index: 2;
  }
}
@media screen and (min-width: 600px) {
  .management1 {
    border-left: 2px solid #e53935;
    border-bottom: 2px solid #e53935;
  }
  .management2 {
    border-right: 2px solid #e53935;
    border-bottom: 2px solid #e53935;
    text-align: end;
  }
  .section1 {
    margin-left: -5%;
    margin-top: auto;
    margin-bottom: auto;
    z-index: 2;
  }
  .section2 {
    margin-right: -5%;
    margin-top: auto;
    margin-bottom: auto;
    z-index: 2;
  }
  .border-top {
    float: right;
  }
}
</style>
