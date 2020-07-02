<template>
  <div>
    <v-app-bar id="AppBar" class="mt-2" dense app flat style="position:fixed">
      <v-toolbar-title>
        <nuxt-link to="/" style="text-decoration: none">
          <v-card flat class=" transparent" height="50">
            <div class="secondary2--text transparent" id="mobile-logo">
              <b>A2A</b>
            </div>
          </v-card>
        </nuxt-link>
      </v-toolbar-title>
      <v-spacer />
      <v-dialog
        v-model="dialog"
        fullscreen
        hide-overlay
        transition="scroll-y-transition"
      >
        <template v-slot:activator="{ on }">
          <v-btn icon id="X" v-on="on" class="mt-1">
            <v-icon large>mdi-text-short</v-icon>
          </v-btn>
        </template>
        <!-- Dialog -->
        <v-card class="white" flat id="D-Card">
          <v-toolbar>
            <v-toolbar-title>
              <nuxt-link to="/" style="text-decoration: none">
                <a id="A2A" @click="dialog = !dialog">
                  <v-card flat class="transparent" height="50">
                    <div class="secondary2--text" id="mobile-logo">
                      <b>A2A</b>
                    </div>
                  </v-card>
                </a>
              </nuxt-link>
            </v-toolbar-title>
            <v-spacer></v-spacer>
            <v-spacer></v-spacer>

            <!-- Close BTN -->
            <v-btn icon @click="dialog = false" id="X" class="mt-1">
              <v-icon large>mdi-close</v-icon>
            </v-btn>
          </v-toolbar>
          <v-card class="white grey--text" width="100%" height="100%" flat>
            <v-row row class="ml-12" id="row">
              <!-- Main Page -->
              <v-col xl="6" lg="6" md="6" sm="12" cols="12" id="Page">
                <!-- Page -->
                <div>
                  <v-col lg="12" v-for="page in Pages" :key="page">
                    <nuxt-link :to="page.link" style="text-decoration: none">
                      <v-flex text id="Btn" @click="dialog = !dialog">
                        {{ page.title }}
                      </v-flex>
                    </nuxt-link>
                  </v-col>
                </div>
              </v-col>

              <v-col xl="4" lg="4" md="6" class="mt-lg-3">
                <!-- Page's Content -->
                <!-- Content -->
                <div id="Content">
                  <v-col lg="12">
                    <h3 class="gray--text Content">BUSINESSES</h3>
                  </v-col>
                  <v-col
                    lg="12"
                    v-for="content in Contents"
                    :key="content.title"
                    id="Contents"
                  >
                    <nuxt-link :to="content.link" class="subTitleLink">
                      <h4
                        class="font-weight-light L-Btn"
                        id="subTitle"
                        @click="dialog = !dialog"
                      >
                        {{ content.name }}
                      </h4>
                    </nuxt-link>
                  </v-col>
                </div>

                <!-- Contacts -->
              </v-col>

              <!-- Link -->
              <v-col xl="2" lg="2" md="12" sm="12" cols="12">
                <div id="Link">
                  <v-row>
                    <v-col
                      lg="12"
                      xl="12"
                      md="1"
                      sm="2"
                      cols="2"
                      v-for="link in links"
                      :key="link"
                    >
                      <a
                        :href="link.link"
                        style="text-decoration: none"
                        target="_blank"
                      >
                        <v-btn icon class="L-Btn ml-6 mb-12" :id="link.id">
                          <v-icon>{{ link.icon }}</v-icon>
                        </v-btn>
                      </a>
                    </v-col>
                  </v-row>
                </div>
              </v-col>
            </v-row>
          </v-card>
        </v-card>
      </v-dialog>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  data: () => ({
    dialog: false,

    // Page
    Pages: [
      {
        title: 'About',
        link: '/about'
      },
      {
        title: 'Careers',
        link: '/career'
      },
      {
        title: 'Blog',
        link: '/blog'
      },
      {
        title: 'News',
        link: '/news'
      },
      {
        title: 'Contact',
        link: '/contact'
      }
    ],

    // Content
    Contents: [
      {
        link: '/business/a2aDigital',
        name: 'A2A Digital'
      },
      {
        link: '/business/property',
        name: 'Property development'
      },
      {
        link: '/business/kit',
        name: 'Kirirom Institute of Technology'
      },
      {
        link: '/business/vKirirom',
        name: 'vKirirom Pine Resort'
      }
    ],

    // Contact
    Direction:
      'https://www.google.com/maps/dir//vKirirom+Head+Office,+Phnom+Penh/@11.5615069,104.855044,17z/data=!4m8!4m7!1m0!1m5!1m1!1s0x310951ce9bbfc447:0x47ac1cdb64ace078!2m2!1d104.857238!2d11.5615069',
    Contacts: [
      {
        email: 'info@asiato.asia',
        tel: ' + (855) 78 777 384',
        location:
          ' House #12, street 2001, Poprak Thbong Village, Sangkat Kakab 1, Khan Posenchey, Phnom Penh.'
      }
    ],

    // Link
    links: [
      {
        icon: 'mdi-linkedin ',
        id: 'LinkedIn',
        link: 'https://www.linkedin.com/company/a2adigital/about/'
      },
      {
        icon: 'mdi-facebook',
        id: 'Facebook',
        link: 'https://www.facebook.com/a2adigitalcambodia/'
      },
      {
        icon: 'mdi-twitter',
        id: 'Twitter',
        link: 'https://twitter.com/a2adigital'
      }
    ]
  }),
  methods: {}
}
</script>

<style scoped lang="scss">
#mobile-logo {
  font-size: 25px;
  display: block;
  position: relative;
  margin-top: 15px;
  margin-left: 20px;
}
#Logo {
  height: 55px;
  width: 45px;
}
#AppBar {
  background-color: transparent;
}
#X {
  transition: 1s;
}
#X:hover {
  position: relative;
  margin-right: 10px;
}
.Location {
  color: #424242;
  transition: 1s;
}
.Location:hover {
  color: black;
  margin-left: 10px;
}
#A2A {
  transition: 1s;
}
#A2A:hover {
  position: relative;
  margin-top: 100px;
}
#D-Card {
  overflow: hidden;
}
.a2aLink {
  text-decoration: none;
}
#Contacts {
  position: relative;
  left: -2%;
}
/* pAGE */
#Btn {
  color: grey;
  font-size: 50px;
  height: 70px;
}
#Btn:hover {
  color: black;
}
/*  */

/* Content */
#Contents :hover {
  color: gray;
}

.subTitleLink {
  text-decoration: none;
  color: grey;
}
#subTitle {
  color: black;
}
.content {
  color: #424242;
}
/* Link */
.Btn {
  background-color: white;
}
#Instagram:hover {
  color: white;
  background-color: RGB(225, 48, 108);
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
@media only screen and (max-width: 960px) {
  #Btn {
    font-size: 40px;
    height: 40px;
  }
  #Contact {
    display: none;
  }
}
@media only screen and (max-width: 600px) {
  #Contents {
    position: relative;
    margin-left: 15px;
  }
  #Btn {
    height: 35px;
    font-size: 35px;
  }
  #subTitle {
    height: 25px;
  }
  #Logo {
    display: none;
  }
  #mobile-logo {
    font-size: 20px;
    display: block;
    position: relative;
    margin-top: 15px;
    margin-left: 5px;
  }
  #AppBar {
    position: relative;
    top: -2%;
    background-color: white;
  }
  .Content {
    position: relative;
    left: -10px;
  }
  .L-Btn {
    position: relative;
    left: -25px;
  }
  #Page {
    padding: 0%;
    margin: 0%;
    position: relative;
    left: 0%;
  }
  #Link {
    position: relative;
    top: -25px;
  }
}

/* Animation  */

#Page {
  animation-name: slideInLeft;
  animation-duration: 1s;
  animation-delay: 0;
}
#Contact {
  animation-name: slideInRight;
  animation-duration: 1s;
  animation-delay: 0;
}
#Link,
#Content {
  animation-name: slideInDown;
  animation-duration: 1s;
  animation-delay: 0;
}
@keyframes slideInLeft {
  from {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    visibility: visible;
  }

  to {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
  }
}
@keyframes slideInRight {
  from {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    visibility: visible;
  }

  to {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
  }
}
@keyframes slideInDown {
  from {
    -webkit-transform: translate3d(0, -100%, 0);
    transform: translate3d(0, -100%, 0);
    visibility: visible;
  }

  to {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
  }
}
</style>
