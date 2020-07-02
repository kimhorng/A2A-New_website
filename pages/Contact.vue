<template>
  <div>
    <v-container>
      <v-row class="mt-6">
        <v-col
          xl="6"
          lg="6"
          md="6"
          sm="12"
          cols="12"
          class="px-12 hidden-sm-and-up"
        >
          <img
            src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766600/A2A%20Image/vector_whrfrg_nbbhnk.jpg"
            class="img-responsive ml-12"
            max-width="100%"
            alt="vector1"
          />
        </v-col>
        <v-col xl="6" lg="6" md="6" sm="6" cols="12">
          <v-card flat class="mt-12">
            <p class="display-1 mt-12">
              What are you looking for?
            </p>
            <p class="headline grey--text">
              Drop us a line
            </p>
            <v-card-action>
              <v-form v-model="isValid">
                <div style="padding-top: 0px; padding-left: 0px">
                  <v-text-field
                    color="red darken-1"
                    label="Subject of interest"
                    v-model="interested"
                    :rules="rules"
                    required
                  />
                </div>
                <div class="ml-3">
                  <v-row>
                    <v-col
                      xl="6"
                      lg="6"
                      md="6"
                      sm="6"
                      cols="12"
                      style="padding-top: 0px; padding-left: 0px"
                    >
                      <v-text-field
                        color="red darken-1"
                        label="Name"
                        v-model="name"
                        :rules="rules"
                        required
                      />
                    </v-col>
                    <v-col
                      xl="6"
                      lg="6"
                      md="6"
                      sm="6"
                      cols="12"
                      style="padding-top: 0px; padding-left: 0px"
                    >
                      <v-text-field
                        color="red darken-1"
                        label="Email"
                        v-model="email"
                        :rules="emailRules"
                        required
                      />
                    </v-col>
                  </v-row>
                </div>
                <div>
                  <v-text-field
                    color="red darken-1"
                    label="Tell us about what you want to know"
                    v-model="projectDescription"
                    :rules="rules"
                    required
                  />
                </div>

                <v-dialog v-model="dialog" persistent max-width="500">
                  <template v-slot:activator="{ on }">
                    <v-card flat width="110" class="mt-6" id="B-Card">
                      <v-container>
                        <v-btn
                          outlined
                          class="secondary2--text"
                          style="left:-15px ; color:"
                          @click.stop="snackbar = true"
                          v-on="on"
                          :disabled="!isValid"
                          id="btn"
                        >
                          SEND REQUEST
                        </v-btn>
                      </v-container>
                    </v-card>
                  </template>
                  <v-card flat height="400">
                    <v-card class="teal accent-3" height="50%" flat>
                      <v-icon color="white" size="100" class="Check"
                        >mdi-check-circle-outline</v-icon
                      >
                    </v-card>
                    <v-card
                      flat
                      height="50%"
                      class="text-center pt-6"
                      color="blue-grey--text darken-4"
                    >
                      <div class="display-1 mb-3">Great!</div>
                      <div class="mb-8">
                        Your information has submitted successfully.
                      </div>
                      <v-btn class="amber white--text" text to="/">
                        Start Exploring
                        <v-icon class="ml-2"> mdi-arrow-right</v-icon>
                      </v-btn>
                    </v-card>
                  </v-card>
                </v-dialog>
              </v-form>
            </v-card-action>
          </v-card>
        </v-col>
        <v-col
          xl="6"
          lg="6"
          md="6"
          sm="6"
          cols="12"
          class="px-12 hidden-xs-only"
        >
          <img
            src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766600/A2A%20Image/vector_whrfrg_nbbhnk.jpg"
            class="img-responsive ml-12"
            style="width:1000px;"
            alt="vector2"
          />
        </v-col>
      </v-row>
    </v-container>
    <section>
      <v-card class="grey lighten-5 text-center pt-12 mt-12" flat height="200">
        <p class="grey--text">Contact us</p>
        <div class="display-1">info@asiato.asia</div>
      </v-card>

      <!--  -->
      <v-card flat class="py-12  mt-3">
        <v-img
          src="https://cuberto.com//assets/img/contacts/alexandria.png"
          width="100"
          class="mx-auto"
          alt="vector3"
        />
        <p class="display-1 mt-2 text-center">Our Location</p>
        <div
          class="grey--text"
          style="width:90% ; margin-right: auto; margin-left: auto ; text-align: center"
        >
          <p>
            <a
              class="grey--text"
              href="https://maps.app.goo.gl/fMCQmV458XwEi1rG6"
              target="_blank"
              style="text-decoration: none"
            >
              Phnom Penh Head Office: House #12, street 2001, Poprak Thbong
              Village, Sangkat Kakab 1, Khan Posenchey, Phnom Penh.</a
            >
          </p>
          <p>
            Office: Plug and Play Shibuya Tokyo-Fudousan, 1-10-8 Dogenzaka
            Shibuya-ku Tokyo Japan
          </p>
          <p>Postal Code: 150-0043</p>
          <p>+855 12 345 678</p>
          <p>vKirirom Japan Inc.</p>

          <v-btn
            outlined
            width="200"
            :href="Direction"
            class="Location secondary2--text mt-6"
            target="_blank"
            id="btn"
          >
            <span>Get Direction </span>
          </v-btn>
        </div>
      </v-card>
    </section>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Footer from '../layouts/Footer'
export default {
  components: {
    Footer
  },
  data: () => ({
    dialog: false,
    interested: '',
    name: '',
    email: '',
    projectDescription: '',
    snackbar: false,
    isValid: false,

    rules: [v => !!v || 'required!'],
    emailRules: [
      v => !!v || 'Email is required',
      v =>
        /.+@.+/.test(v) || 'E-mail must be valid, Example: username@gmail.com'
    ]
  })
}
</script>

<style scoped>
#btn {
  transition: 1s;
}
#btn:hover {
  margin-left: 10px;
}
.Check {
  top: 25%;
  left: 40%;
}
@media screen and (max-width: 600px) {
  .img-responsive {
    max-width: 100%;
  }
  .Check {
    left: 35%;
  }
}
@media screen and (min-width: 600px) {
  .img-responsive {
    max-width: 100%;
  }
}
@media screen and (min-width: 960px) {
  .img-responsive {
    max-width: 100%;
  }
}
</style>
