<template>
  <section id="welcome" style="height: 100%">
    <v-row style="height: 100%">
      <v-container class="d-flex align-md-center">
        <v-col cols="12" sm="6" md="6" class="d-flex flex-column">
          <div class="notice-box text-center">WE’RE HIRING!</div>

          <div class="welcome-text" v-text="welcome.text" />

          <nuxt-link to="/career">
            <div class="goto-careers d-flex align-center">
              <span class="mr-3">Go to Careers</span>
              <v-icon size="16px" color="#bd182a">mdi-arrow-right</v-icon>
            </div>
          </nuxt-link>
          <div>
            <a @click="onScrolled">
              <img
                src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766597/A2A%20Image/scroll2_dn1jlb_envrhx.jpg"
                style="width: 85px ; height: 47px;"
                id="S-Img"
                alt="Scroll-img"
              />
            </a>
          </div>
        </v-col>

        <v-col
          cols="12"
          sm="6"
          md="6"
          class="welcome-img-box d-flex justify-end align-end"
          style="padding: 0px"
        >
          <v-img
            class="welcome-img"
            src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766604/A2A%20Image/welcome1-min_t59yyl_nd7ym4.jpg"
            alt="welcome-img"
          ></v-img>
        </v-col>
      </v-container>
    </v-row>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      welcome: {
        text:
          'Respect, Professionalism, Excellence, Innovation and creativity, Independent thinking.'
      }
    }
  },
  methods: {
    onScrolled() {
      fullpage_api.moveSectionDown()
    }
  }
}
</script>

<style scoped lang="scss">

#S-Img {
  transition: 1s;
}
#S-Img:hover {
  margin-left: 10px;
}
@media screen and (min-width: 960px) {
  .welcome-img {
    max-width: 600px;
  }
  #S-Img{
    margin-top:40%
  }
}

@media screen and (min-width: 600px) {
  #welcome {
    padding-top: 56px;

    .container {
      padding: 25px;

      .notice-box {
        margin-top: 36px;
        background-color: #bd182a;
        color: white;
        width: 144px;
        margin-bottom: 36px;
        border-radius: 2px;
      }

      .welcome-text {
        font-weight: 200;
        font-size: 27px;
        line-height: 150%;
        margin-bottom: 36px;
      }

      .goto-careers {
        color: #bd182a;
        font-weight: 500;
        font-size: 16px;
      }

      .welcome-img-box {
        position: absolute;
        right: 0;
        bottom: 0;
      }
    }
  }
  #S-Img{
    margin-top:40%
  }
}

@media screen and (max-width: 600px) {
  .welcome-img {
    max-width: 230px;
  }
  #S-Img{
    margin-top:40%;
  }
  #welcome {
    padding-top: 56px;

    .container {
      padding: 25px;

      .notice-box {
        margin-top: 36px;
        background-color: #bd182a;
        color: white;
        width: 144px;
        margin-bottom: 36px;
      }

      .welcome-text {
        font-weight: 200;
        font-size: 27px;
        line-height: 150%;
        margin-bottom: 36px;
      }

      .goto-careers {
        color: #bd182a;
        font-weight: bold;
        font-size: 14px;
      }

      .welcome-img-box {
        position: absolute;
        right: 0;
        bottom: 0;
      }
    }
  }
}

@media screen and (max-width: 375px) {
  .welcome-img {
    max-width: 200px;
    margin-top: -20px;
  }
  #S-Img{
    margin-top:40%
  }

  #welcome {
    padding-top: 20px;

    .container {
      padding: 25px;

      .notice-box {
        margin-top: 36px;
        background-color: #bd182a;
        color: white;
        width: 144px;
        margin-bottom: 36px;
      }

      .welcome-text {
        font-weight: 200;
        font-size: 20px;
        line-height: 150%;
        margin-bottom: 36px;
      }

      .goto-careers {
        color: #bd182a;
        font-weight: bold;
        font-size: 14px;
      }

      .welcome-img-box {
        position: absolute;
        right: 0;
        bottom: 0;
      }
    }
  }
}

@media screen and (max-width: 320px) {
  .welcome-img {
    max-width: 200px;
    margin-top: -20px;
  }
  #S-Img{
    margin-top:30%
  }

  #welcome {
    padding-top: 20px;

    .container {
      padding: 25px;

      .notice-box {
        margin-top: 36px;
        background-color: #bd182a;
        color: white;
        width: 144px;
        margin-bottom: 36px;
      }

      .welcome-text {
        font-weight: 200;
        font-size: 20px;
        line-height: 150%;
        margin-bottom: 36px;
      }

      .goto-careers {
        color: #bd182a;
        font-weight: bold;
        font-size: 14px;
      }

      .welcome-img-box {
        position: absolute;
        right: 0;
        bottom: 0;
      }
    }
  }
}
</style>
