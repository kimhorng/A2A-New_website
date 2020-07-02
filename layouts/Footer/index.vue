<template>
  <div>
    <hr
      width="100%"
      style="height: 3px ; color:#F4F5F7 ;background-color: #F4F5F7 ;"
    />
    <section class="pt-8">
      <v-container style="padding-bottom: 0px;">
        <v-row>
          <v-col sm="6" md="3" cols="6">
            <div>
              <h2 class="mb-4 secondary2--text" style="margin-top: -25px">
                Company
              </h2>
              <nuxt-link
                to="/"
                class="black--text"
                style="text-decoration: none"
              >
                <p>Home</p>
              </nuxt-link>
              <nuxt-link
                to="/about"
                class="black--text"
                style="text-decoration: none"
              >
                <p style="margin-top: -20px">About</p>
              </nuxt-link>
              <nuxt-link
                to="/career"
                class="black--text"
                style="text-decoration: none"
              >
                <p style="margin-top: -20px">Careers</p>
              </nuxt-link>
              <nuxt-link
                to="/blog"
                class="black--text"
                style="text-decoration: none"
              >
                <p style="margin-top: -20px">Blog</p>
              </nuxt-link>
              <nuxt-link
                to="/news"
                class="black--text"
                style="text-decoration: none"
              >
                <p style="margin-top: -20px">News</p>
              </nuxt-link>
            </div>
          </v-col>
          <v-col sm="6" md="3" cols="6">
            <div>
              <h2 class="mb-4 secondary2--text" style="margin-top: -25px">
                Businesses
              </h2>

              <nuxt-link
                to="/business/a2aDigital"
                class="black--text"
                style="text-decoration: none"
              >
                <p>A2A Digital</p>
              </nuxt-link>

              <nuxt-link
                to="/business/property"
                class="black--text"
                style="text-decoration: none"
              >
                <p style="margin-top: -20px">Property development</p>
              </nuxt-link>

              <nuxt-link
                to="/business/kit"
                class="black--text"
                style="text-decoration: none"
              >
                <p style="margin-top: -20px">Kirirom Institute of Technology</p>
              </nuxt-link>

              <nuxt-link
                to="/business/vkirirom"
                class="black--text"
                style="text-decoration: none"
              >
                <p style="margin-top: -20px">vKirirom Pine Resort</p>
              </nuxt-link>
            </div>
          </v-col>
          <v-col sm="6" md="3" cols="12">
            <div>
              <h2 class="mb-4 secondary2--text" style="margin-top: -25px">
                Contact Us
              </h2>
              <v-row class="pl-2" style="margin-top: -15px"
                ><v-icon class="secondary2--text" small left
                  >mdi-phone-in-talk-outline</v-icon
                >
                <p class="pt-3">+855 (0)95 77 844</p></v-row
              >
              <v-row class="pl-2" style="margin-top: -30px"
                ><v-icon class="secondary2--text" small left
                  >mdi-email-outline</v-icon
                >
                <p class="pt-3">info@asiato.asia</p></v-row
              >
            </div>
          </v-col>
          <v-col sm="6" md="3" cols="12">
            <div>
              <h2 class="mb-4 secondary2--text" style="margin-top: -25px">
                Address
              </h2>
              <div style="font-size: 12px">
                <p style="line-height: 27px; margin-top:20px">
                  <a
                    class="black--text"
                    href="https://maps.app.goo.gl/fMCQmV458XwEi1rG6"
                    target="_blank"
                    style="text-decoration: none"
                  >
                    Phnom Penh Head Office: House #12, street 2001, Poprak
                    Thbong Village, Sangkat Kakab 1, Khan Posenchey, Phnom
                    Penh.</a
                  >
                </p>
                <p style="line-height: 27px; margin-top: -15px ;">
                  Office: Plug and Play Shibuya Tokyo-Fudousan, 1-10-8 Dogenzaka
                  Shibuya-ku Tokyo Japan
                </p>
                <p style="line-height: 27px; margin-top: -15px ">
                  Postal Code: 150-0043
                </p>
                <p style="line-height: 27px; margin-top: -15px ">
                  +855 12 345 678
                </p>
                <p style="line-height: 27px; margin-top: -15px ">
                  vKirirom Japan Inc.
                </p>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </section>
    <section style="background-color: #F4F5F7 ;">
      <v-row style="padding-bottom: 0px ; margin-right:0px; margin-left:0px">
        <v-col sm="4" md="4" cols="12" class="text-center">
          <v-btn text class="secondary1--text headline font-weight-bold" to="/"
            >A2A</v-btn
          >
        </v-col>
        <v-col
          sm="4"
          md="4"
          cols="12"
          class=" text-center"
          style="padding-bottom: 0px"
        >
          <a
            href="https://www.linkedin.com/company/a2adigital/about/"
            target="_blank"
            class="black--text"
            style="text-decoration: none"
          >
            <v-btn icon id="LinkedIn">
              <v-icon>mdi-linkedin</v-icon>
            </v-btn>
          </a>

          <a
            href="https://www.facebook.com/a2adigitalcambodia/"
            target="_blank"
            class="black--text"
            style="text-decoration: none"
          >
            <v-btn icon id="Facebook">
              <v-icon>mdi-facebook</v-icon>
            </v-btn>
          </a>

          <a
            href="https://twitter.com/a2adigital"
            target="_blank"
            class="black--text"
            style="text-decoration: none"
          >
            <v-btn icon id="Twitter">
              <v-icon>mdi-twitter</v-icon>
            </v-btn>
          </a>
        </v-col>

        <v-col
          sm="4"
          md="4"
          cols="12"
          class="copyright"
          style="padding-bottom: 0px"
        >
          <p
            style="font-size: 12px ; padding-bottom: 0px; margin-bottom: 0px;"
            class="text-center"
          >
            Copyright &copy; 2020 A2A Town(Cambodia) Co.ltd.
          </p>
        </v-col>
      </v-row>
    </section>
  </div>
</template>

<script>
export default {}
</script>

<style>
.Btn {
  background-color: white;
}
#Twitter:hover {
  color: white;
  background-color: RGB(29, 161, 242);
}
#Facebook:hover {
  color: white;
  background-color: RGB(59, 89, 152);
}
#LinkedIn:hover {
  color: white;
  background-color: RGB(40, 103, 178);
}
@media screen and (max-width: 600px) {
  .copyright {
    margin-top: -10px;
  }
}
</style>
