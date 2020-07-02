<template>
  <div>
    <div class="hidden-xs-only">
      <section>
        <v-container>
          <v-row wrap class="mt-12 mb-12">
            <v-col cols="12" sm="6" md="6" class="my-auto">
              <h2 id="Title">A2A Construction</h2>
            </v-col>

            <v-col cols="12" sm="6" md="6" class="my-auto">
              <p id="Sub" class="pt-5">Invest on your vacation home in the nature</p>
            </v-col>
          </v-row>
        </v-container>
      </section>

      <section>
        <v-row id="Background">
          <v-col id="Img" class="bg" alt="background"> </v-col>
        </v-row>
      </section>

      <section class="all_text" style="background-color: #fafafa">
        <v-container>
          <v-row wrap class="mx-auto">
            <v-col cols="10" class="pr-md-12 mx-auto" id="Text">
              <div class="mt-12 mb-12">
                <h2>
                  About Real Estate
                </h2>
                <p class="pt-4">
                  vKirirom is nestled amongst the rare pine trees in Kirirom
                  National Park on a mountain 700 meters above sea level. Our
                  duty is to develop ecotourism by making it accessible to many
                  visitors while protecting its beauty for many generations to
                  come through eco-friendly sustainable development.
                </p>
                <p class="pt-4">
                  The weather and natural beauty of Kirirom will create a
                  perfect environment for entrepreneurs, residents, and students
                  seeking a living and working space for creativity, health, and
                  innovation. vKirirom Nature will be integrated with bespoke IT
                  technologies created by KIT University - a major driver of
                  innovation-focused economy to be developed to become the
                  Silicon Valley of Southeast Asia.
                </p>

                <h2 class="pt-4">
                  vKirirom Property Lease and Investment Characteristics
                </h2>
                <ul class="pt-4">
                  <li>9 year leaseback guarantee</li>
                  <li>2062 year lease with first renewal rights</li>
                  <li>Build homes to fulfill annual student growth</li>
                  <li>
                    Fully maintained with no hidden cost during the leaseback
                    period
                  </li>
                </ul>

                <!-- Type R -->
                <h2 class="pt-4">
                  1FL Standalone villa (Type R)
                </h2>
                <p class="pt-4">
                  Perfect for the social investor who seeks to help our
                  Cambodian sponsorship students as well as a solid and steady
                  ROI. In the future after the leaseback period, the standalone
                  villa is ideal as 2nd home as the resort continues to expand
                  into a large nature community.
                </p>
                <!-- Img -->
                <v-carousel
                  cycle
                  height="400"
                  hide-delimiter-background
                  show-arrows-on-hover
                  class="red"
                >
                  <v-carousel-item v-for="typeR in TypeR" :key="typeR">
                    <v-sheet height="100%">
                      <v-row
                        class="fill-height"
                        align="center"
                        justify="center"
                      >
                        <v-img
                          :src="typeR.src"
                          alt="Type A's Villa"
                          contain
                          height="100%"
                        />
                      </v-row>
                    </v-sheet>
                  </v-carousel-item>
                </v-carousel>
                <!-- <v-img></v-img> -->

                <h3 class="pt-4">Property Information</h3>
                <b>Building Type: </b> 1FL Stand-alone Villa <br />
                <b>Building Footprint:</b> 36 square meters<br />
                <b>Land Size:</b> ~200 square meters <br />
                <b>Maintances: </b>All inc. during leasback period <br />

                <h3 class="mt-5 pt-4">Investment Informations:</h3>
                <b>Type:</b> Student Dorm Leas eback <br />
                <b>Annual Leaseback(Gross): </b> $3,300/7 free nights <br />
                <b>Total Price:</b> $55,000(inc. VAT, funiture)

                <!-- Type A -->
                <h2 class="mt-5 pt-4">
                  Upscale Resort Villa with Rooftop Garden (Type A) <br />
                </h2>
                <p class="pt-4">
                  Perfect for the investor with a large family or likes to
                  entertain who also seeks a steady ROI through our resort
                  leaseback plan. Investors can enjoy two weeks per year in this
                  gorgeous 3 bedroom villa and impress friends with a rooftop
                  garden BBQ party. In the future after the leaseback period,
                  the standalone villa is ideal as 2nd vacation home or even
                  retirement home as the resort expands into a large nature
                  community.
                </p>

                <!-- Img -->
                <v-carousel
                  cycle
                  height="400"
                  hide-delimiter-background
                  show-arrows-on-hover
                  class="red"
                >
                  <v-carousel-item v-for="typeA in TypeA" :key="typeA">
                    <v-sheet height="100%">
                      <v-row
                        class="fill-height"
                        align="center"
                        justify="center"
                      >
                        <v-img
                          :src="typeA.src"
                          alt="Type A's Villa"
                          contain
                          height="100%"
                        />
                      </v-row>
                    </v-sheet>
                  </v-carousel-item>
                </v-carousel>
                <!-- <v-img></v-img> -->

                <h3 class="pt-4 mt-4">Property Information</h3>
                <b>Building Type: </b> 2FL 3 Bedrooms Villa <br />
                <b>Land Size:</b> ~600 square meters<br />
                <b>Building Footprint:</b> 114 square meters<br />
                <b>Maintances: </b>All inc. during leasback period <br />

                <h3 class="mt-5 pt-4">Investment Informations:</h3>
                <b>Type:</b> Student Dorm Leas eback <br />
                <b>Annual Leaseback(Gross): </b> $9,000/14 free nights <br />
                <b>Total Price:</b> $185,000(inc. VAT, funiture, Rooftop garden)

                <!-- Type V -->
                <h2 class="mt-5 pt-4">
                  Modern Condo with Private Garden or Balcony ( Type V )
                </h2>
                <p class="pt-4">
                  Perfect for the social investor who seeks to help our
                  Cambodian sponsorship students as well as a solid and steady
                  ROI. In the future after the leaseback period, the modern
                  condo is ideal as 2nd home as the resort continues to expand
                  into a large nature community.
                </p>

                <!-- Img -->
                <v-carousel
                  cycle
                  height="400"
                  hide-delimiter-background
                  show-arrows-on-hover
                  class="red"
                >
                  <v-carousel-item v-for="typeV in TypeV" :key="typeV">
                    <v-sheet height="100%">
                      <v-row
                        class="fill-height"
                        align="center"
                        justify="center"
                      >
                        <v-img
                          :src="typeV.src"
                          alt="Type A's Villa"
                          contain
                          height="100%"
                        />
                      </v-row>
                    </v-sheet>
                  </v-carousel-item>
                </v-carousel>
                <!-- <v-img></v-img> -->

                <h3 class="pt-4 mt-4">Property Information</h3>
                <b>Building Type: </b> Condo <br />
                <b>Building Footprint:</b> 45 square meters<br />
                <b>Land Size:</b> ~146 square meters <br />
                <b>Maintances: </b>All inc. during leasback period <br />

                <b>Land Size:</b> ~146 square meters

                <h3 class="mt-5 pt-4">Investment Informations:</h3>
                <b>Type:</b> Student Dorm Leas eback <br />
                <b>Annual Leaseback(Gross): </b> $4,350/7 free nights <br />
                <b>Total Price:</b> $65,000(inc. VAT, funiture)

                <!-- Type L -->
                <h2 class="mt-5 pt-4">
                  2Fl Share House Villa (Type L)
                </h2>
                <p class="pt-4">
                  Perfect for the large social investor who seeks to help our
                  Cambodian sponsorship students as well as a high and steady
                  ROI. In the future after the leaseback period, this 2Fl shared
                  house design is perfect as a rental property for digital
                  nomads who are expected to be a major part of our growing
                  nature community.
                </p>

                <!-- Img -->
                <v-carousel
                  cycle
                  height="400"
                  hide-delimiter-background
                  show-arrows-on-hover
                  class="red"
                >
                  <v-carousel-item v-for="typeL in TypeL" :key="typeL">
                    <v-sheet height="100%">
                      <v-row
                        class="fill-height"
                        align="center"
                        justify="center"
                      >
                        <v-img
                          :src="typeL.src"
                          alt="Type A's Villa"
                          contain
                          height="100%"
                        />
                      </v-row>
                    </v-sheet>
                  </v-carousel-item>
                </v-carousel>
                <!-- <v-img></v-img> -->

                <h3 class="pt-4 mt-4">Property Information</h3>
                <b>Building Type: </b> 2Fl Stand-alone Villa <br />
                <b>Building Footprint:</b> 123 square meters<br />
                <b>Land Size:</b> ~600 square meters<br />
                <b>Maintances: </b>All inc. during leasback period <br />

                <h3 class="mt-5 pt-4">Investment Informations:</h3>
                <b>Type:</b> Student Dorm Leas eback <br />
                <b>Annual Leaseback(Gross): </b> $26,000/14 free nights <br />
                <b>Total Price:</b> $305,000(inc. VAT, funiture)

                <!-- Type S -->

                <h2 class="mt-5 pt-4">
                  2Fl Party Townhouse with Community Pool BBQ Space (Type S)
                </h2>
                <p class="pt-4">
                  Perfect for people seeking a high quality of life and likes to
                  host friends and family at this 2FL townhouse designed for
                  entertaining. House is part of a larger community with a
                  shared pool and BBQ space with an outdoor entertainment area
                  reserved just for this exclusive community. Ideal as a future
                  retirement home as the resort grows into a large nature
                  community ideal for living, working, and playing.
                </p>
                <v-carousel
                  cycle
                  height="400"
                  hide-delimiter-background
                  show-arrows-on-hover
                  class="red"
                >
                  <v-carousel-item v-for="typeS in TypeS" :key="typeS">
                    <v-sheet height="100%">
                      <v-row
                        class="fill-height"
                        align="center"
                        justify="center"
                      >
                        <v-img
                          :src="typeS.src"
                          alt="Type A's Villa"
                          contain
                          height="100%"
                        />
                      </v-row>
                    </v-sheet>
                  </v-carousel-item>
                </v-carousel>
                <h4 class="pt-4">Concept:</h4>
                Spend quality time with family and friends in your 2nd home
                amongst the pine trees. Enjoy healthy lifestyle in cool mountain
                air. Invite friends to community pool with shared BBQ space for
                fun and relaxing parties to create forever memories.<br />
                <h3 class="pt-4">Property Information</h3>
                <b>Building Footprint:</b> 68 square meters<br />
                <b>Maintances: </b>$600/Year<br />
                <b>Building Type: </b> 2Fl Townhouse (Duplex) <br />
                <b>Land Size:</b> ~300 square meters <br />
                <b>Total Price: </b> $120,000 (inc. VAT, no funiture)
              </div>
            </v-col>
          </v-row>
        </v-container>
      </section>

      <section class="each_link">
        <v-row style="height: 100%">
          <v-flex class="my-auto">
            <div class="text-center">
              <a
                href="https://vkirirom.com/listing/nature-city-investment-cambodia-property"
                target="_blank"
                id="btn" style="text-decoration:none"
              >
                <v-btn width="200px" primary light outlined class="mx-auto secondary1--text text-capitalize">
                  <span class="title">Lease a Property</span>
                </v-btn>
              </a>
            </div>
          </v-flex>
        </v-row>
      </section>
      <section class="footer">
        <div class="img_responsive">
          <nuxt-link to="/business/vkirirom" class="link">
            <div class="last_img">
              <v-row class="blur">
                <v-flex class="my-auto">
                  <div class="text-center">
                    <p class="display-1">Next Project</p>
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
          <property />
        </v-carousel-item>

        <v-carousel-item>
          <vkirirom />
        </v-carousel-item>

        <v-carousel-item>
          <a2aDigital />
        </v-carousel-item>

        <v-carousel-item>
          <kit />
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
  },
  data: () => ({
    TypeA: [
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766869/Properties/Type_A_1-min_ovccde_yuxowx.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766863/Properties/Type_A_2-min_ifoivr_jsveyt.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766863/Properties/Type_A_3-min_hnicxu_k4bxqc.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766864/Properties/Type_A_4-min_hrwafy_l6rigc.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766863/Properties/Type_A_5-min_wjux69_cv00ax.jpg'
      }
    ],
    TypeV: [
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766867/Properties/Type_V_1-min_fb01u5_whcowi.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766868/Properties/Type_V_2-min_ntgyvf_bdhncc.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766868/Properties/Type_V_3-min_acnxdv_p1oeek.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766868/Properties/Type_V_4-min_iwy3s4_kxzooy.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766868/Properties/Type_V_5-min_xu1rvo_e2hed5.jpg'
      },
    ],
    TypeS: [
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766866/Properties/Type_S_1-min_kd1e9c_zihxrz.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766866/Properties/Type_S_2-min_glkxiv_wabd2p.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766866/Properties/Type_S_3-min_gfv88b_dpmmvr.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766867/Properties/Type_S_4-min_v9iiap_hzr2si.jpg'
      }
    ],
    TypeL: [
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766863/Properties/Type_L_1-min_yg6xwg_jbkxxz.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766864/Properties/Type_L_2-min_ltddf2_zp4zde.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766864/Properties/Type_L_3-min_vu5rgt_f66qil.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766864/Properties/Type_L_4-min_cbtexf_m0vjen.jpg'
      }
    ],
    TypeR: [
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766865/Properties/Type_R_1-min_tnb96p_qjory2.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766865/Properties/Type_R_2-min_penv5r_lp9oit.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766865/Properties/Type_R_3-min_k7yjem_ihprlw.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766865/Properties/Type_R_4-min_ukmeqf_assscv.jpg'
      },
      {
        src:
          'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766866/Properties/Type_R_5-min_xhxlzu_ra6zmj.jpg'
      }
    ]
  })
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
  .each_link {
    height: 400px;
  }
  .footer {
    height: 400px;
  }
  .last_img {
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591939083/Homepage/vkirirom_res_1_mwjolw.jpg');
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
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766595/A2A%20Image/a2a_construction-min_vcpdbc_k6j5sx.jpg');
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
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591939083/Homepage/vkirirom_res_1_mwjolw.jpg');
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
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766595/A2A%20Image/a2a_construction-min_vcpdbc_k6j5sx.jpg');
    background-size: 100%, 100%, 100%, cover;
  }
}
</style>
