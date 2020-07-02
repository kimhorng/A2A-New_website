<template>
  <div class="mt-12">
    <section>
      <v-container>
        <v-row wrap class="mx-auto">
          <v-col cols="12" xs="12" sm="12" md="6">
            <h2 id="Title">A2A Construction</h2>
          </v-col>

          <v-col cols="12" xs="12" sm="12" md="6">
            <p id="Sub" style="margin-top: -15px">Invest on your vacation home in the nature</p>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <section>
      <v-row id="Background">
        <v-col class="bg" id="Img" alt="background"></v-col>
      </v-row>
    </section>

    <section>
      <v-row wrap class="mx-auto">
        <v-col cols="12" class="pr-md-12 mx-auto info" id="Text">
          <div class="mt-12 mb-12 ">
            <v-container>
              <h2>
                About Real Estate
              </h2>
              <p class="pt-4">
                vKirirom is nestled amongst the rare pine trees in Kirirom
                National Park on a mountain 700 meters above sea level. Our duty
                is to develop ecotourism by making it accessible to many
                visitors while protecting its beauty for many generations to
                come through eco-friendly sustainable development.
              </p>
              <p class="pt-4">
                The weather and natural beauty of Kirirom will create a perfect
                environment for entrepreneurs, residents, and students seeking a
                living and working space for creativity, health, and innovation.
                vKirirom Nature will be integrated with bespoke IT technologies
                created by KIT University - a major driver of innovation-focused
                economy to be developed to become the Silicon Valley of
                Southeast Asia.
              </p>

              <h2 class="pt-4">
                vKirirom Property Lease and Investment Characteristics
              </h2>
              <ul>
                <li>9 year leaseback guarantee</li>
                <li>2062 year lease with first renewal rights</li>
                <li>Build homes to fulfill annual student growth</li>
                <li>
                  Fully maintained with no hidden cost during the leaseback
                  period
                </li>
              </ul>

              <h2 class="pt-4">
                Standalone villa (Type R)
              </h2>
              <p class="pt-4">
                Perfect for the social investor who seeks to help our Cambodian
                sponsorship students as well as a solid and steady ROI. In the
                future after the leaseback period, the standalone villa is ideal
                as 2nd home as the resort continues to expand into a large
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
                <v-carousel-item v-for="typeR in TypeR" :key="typeR">
                  <v-sheet height="100%">
                    <v-row class="fill-height" align="center" justify="center">
                      <v-img
                        :src="typeR.src"
                        alt="Type R's Villa"
                        contain
                        height="100%"
                      />
                    </v-row>
                  </v-sheet>
                </v-carousel-item>
              </v-carousel>
              <!-- <v-img></v-img> -->

              <h3 class="pt-4 mt-4">Property Information</h3>
              <b>Building Type: </b> 1FL Stand-alone Villa <br />
              <b>Building Footprint:</b> 36 square meters<br />
              <b>Land Size:</b> ~200 square meters <br />
              <b>Maintances: </b>All inc. during leasback period <br />

              <h3 class="mt-5">Investment Informations:</h3>
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
                garden BBQ party. In the future after the leaseback period, the
                standalone villa is ideal as 2nd vacation home or even
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
                    <v-row class="fill-height" align="center" justify="center">
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
                Modern Condo with Private Garden or Balcony (Type V)
              </h2>
              <p class="pt-4">
                Perfect for the social investor who seeks to help our Cambodian
                sponsorship students as well as a solid and steady ROI. In the
                future after the leaseback period, the modern condo is ideal as
                2nd home as the resort continues to expand into a large nature
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
                <v-carousel-item v-for="typeV in TypeV" :key="typeV">
                  <v-sheet height="100%">
                    <v-row class="fill-height" align="center" justify="center">
                      <v-img
                        :src="typeV.src"
                        alt="Type V's Villa"
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

              <h2 class="mt-5 pt-4">
                2Fl Share House Villa (Type L)
              </h2>
              <p class="pt-4">
                Perfect for the large social investor who seeks to help our
                Cambodian sponsorship students as well as a high and steady ROI.
                In the future after the leaseback period, this 2Fl shared house
                design is perfect as a rental property for digital nomads who
                are expected to be a major part of our growing nature community.
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
                    <v-row class="fill-height" align="center" justify="center">
                      <v-img
                        :src="typeL.src"
                        alt="Type L's Villa"
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
                entertaining. House is part of a larger community with a shared
                pool and BBQ space with an outdoor entertainment area reserved
                just for this exclusive community. Ideal as a future retirement
                home as the resort grows into a large nature community ideal for
                living, working, and playing.
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
                    <v-row class="fill-height" align="center" justify="center">
                      <v-img
                        :src="typeS.src"
                        alt="Type S's Villa"
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
              <b>Building Type: </b> 2Fl Townhouse (Duplex) <br />
              <b>Building Footprint:</b> 68 square meters<br />
              <b>Land Size:</b> ~300 square meters <br />
              <b>Maintances: </b>$600/Year<br />
              <b>Total Price: </b> $120,000 (inc. VAT, no funiture)
            </v-container>
          </div>
        </v-col>
      </v-row>
    </section>

    <section>
      <div class="text-center nextProject ">
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
      <div>
        <nuxt-link to="/business/vkirirom" class="link">
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

<script>
export default {
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
h2{
  line-height: 40px;
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
  background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591030698/Homepage/vkirirom_res-min_b8aw6o.jpg');
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
  background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766595/A2A%20Image/a2a_construction-min_vcpdbc_k6j5sx.jpg');
  background-size: cover;
  height: 400px;
}
</style>
