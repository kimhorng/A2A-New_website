<template>
  <full-page id="fullpage" ref="fullpage">
    <div class="section">
      <HomeScreen />
    </div>
    <div v-for="item in items" :key="item.property" class="section">
      <div
        id="business"
        class="img-light hidden-sm-and-up"
        style="height: 100%; width: 100%;"
        v-bind:style="{ backgroundImage: 'url(' + item.src + ')' }"
      >
        <v-row class="mobile_text" style="height: 100%" align="center">
          <v-container style="height: 100%" class="d-flex align-center">
            <v-col >
              <div class="notice-box text-center d-none d-sm-block">
                BUSINESS
              </div>
              <div >
                <div class="business-title">{{ item.title }}</div>
                <div class="business-desc">{{ item.small_tags }}</div>
                <div class="business-tags">{{ item.small_text }}</div>
              </div>
            </v-col>
          </v-container>
        </v-row>

        <v-fab-transition>
          <v-btn
            fab
            absolute
            bottom
            right
            color="#fff"
            class="info-button"
            :to="item.link"
          >
            <v-icon v-text="infoButtonIcon"></v-icon>
          </v-btn>
        </v-fab-transition>
      </div>

      <div
        id="business"
        class="img-light hidden-xs-only"
        style="height: 100%; width: 100%;"
      >
        <v-row wrap style="height: 100%" align="center">
          <v-container style="height: 100%" class="d-flex align-center">
            <v-col sm="6" class="pr-12">
              <div
                class="notice-box text-center d-none d-sm-block"
                style="width:200px; height:35px"
              >
                FEATURE BUSINESS
              </div>
              <div>
                <div class="business-title">{{ item.title }}</div>
                <div class="business-desc">{{ item.desc }}</div>
                <div class="business-tags">{{ item.tags }}</div>
              </div>

              <v-btn
                outlined
                width="150px"
                style="margin-top: 30%"
                flat
                class="subtitle-2 learnmore secondary2--text"
                :to="item.link"
                id="Learn-Btn"
              >
                LEARN MORE
              </v-btn>
            </v-col>
            <v-col
              sm="6"
              class="business-img-box d-none d-sm-block"
              style="padding: 0; height: 100%; width: 100%"
            >
              <div
                class="business-img"
                style="height: 100%; width: 100% "
                v-bind:style="{ backgroundImage: 'url(' + item.src + ')' }"
              ></div>
            </v-col>
          </v-container>
        </v-row>
      </div>
    </div>
  </full-page>
</template>

<script>
import HomeScreen from '../pages/NewHomePage/index'
export default {
  components: {
    HomeScreen
  },
  data: () => ({
    infoButtonIcon: 'mdi-chevron-right',
    items: [
      {
        title: 'A2A Digital',
        desc:
          'Leading digital agency with solid design and development expertise.',
        tags: 'Branding, design, development, product',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766596/A2A%20Image/a2a_digital1-min_ec5j4q_vufkpw.jpg',
        link: '/business/a2adigital',
        small_tags:
          'Cloud Computing, AI, IoT, Blockchain, RPA, ERP, Cyber Security, Digital Marketing, VR/AR ',
        small_text:
          'Providing IT services and building sophisticated applications with cutting edge technologies.'
      },

      {
        title: 'Kirirom Institute of Technology',
        desc:
          'Cambodia’s first boarding technology institute with international standards',
        tags:
          'Tech institute, full-tuition sponsorships, free internships, job placement in abroad',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1591030689/Homepage/kit2-min_z1chdq.jpg',
        link: '/business/kit',
        small_tags:
          'Tech institute, full-tuition sponsorships, free internships, job placement in abroad',
        small_text:
          'An innovative tech institute providing life-changing opportunites and building future leaders. '
      },

      {
        title: 'A2A Construction',
        desc:
          'vKirirom is nestled amongst the rare pine trees in Kirirom National Park on a mountain 700 meters above sea level.',
        tags: 'Comunity pool, upscale villa, modern condo',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766601/A2A%20Image/a2a_construction1-min_eq8fh7_lwiubr.jpg',
        link: '/business/property',
        small_tags:
          'Comunity pool, upscale villa, modern condo, perfect weather',
        small_text:
          'vKirirom is nestled amongst the rare pine trees in Kirirom National Park on a mountain 700 meters above sea level.'
      },

      {
        title: 'Vkirirom Pine Resort',
        desc: "A new concept for enriching people's lives in the future",
        tags: 'Resort, activity, camping, new experiences',
        src: 'https://res.cloudinary.com/dgzbxayiq/image/upload/v1591030698/Homepage/vkirirom_res-min_b8aw6o.jpg',
        link: '/business/vkirirom',
        small_tags:
          'Team-building, off-the-beaten track trips, field trips, company retreats',
        small_text:
          'The perfect resort for off-the-beaten-path family vacations, educational field trips, annual company retreats, business travels.'
      }
    ]
  })
}
</script>
<style scoped lang="scss">
#Learn-Btn{
  transition: 1s;
}
#Learn-Btn:hover{
  margin-left: 10px;
}
@media screen and (min-width: 600px) {
  .business-img {
    // background-position: center, 0% 30%, 0% 30%, center;
    // background-size: 100%, contain, contain, cover;
    background-size: contain;
    background-position: 50% 75%;
  }

  #business {
    .notice-box {
      margin-top: 36px;
      background-color: #bd182a;
      color: white;
      width: 144px;
      margin-bottom: 36px;
      border-radius: 2px;
    }

    .business-title {
      font-size: 30px;
      font-weight: 400;
      line-height: 150%;
      color: #000;
      margin-bottom: 32px;
    }

    .business-desc {
      font-size: 24px;
      font-weight: 200;
      line-height: 150%;
      color: #000;
      margin-bottom: 32px;
    }

    .business-tags {
      font-size: 16px;
      font-weight: 400;
      line-height: 150%;
      color: #000;
    }

    .info-button {
      bottom: 0;
      margin-bottom: 24px;
    }

    .business-img-box {
      position: absolute;
      right: 0;
      bottom: 0;
    }
  }
}

@media screen and (min-width: 960px) {
  .business-img {
    background-position: center, 0 70%, 0 70%, center;
    background-size: 100%, 100%, 100%, cover;
  }

  #business {
    .notice-box {
      margin-top: 36px;
      background-color: #bd182a;
      color: white;
      width: 144px;
      margin-bottom: 36px;
      border-radius: 2px;
    }

    .business-title {
      font-size: 30px;
      font-weight: 400;
      line-height: 150%;
      color: #000;
      margin-bottom: 32px;
    }

    .business-desc {
      font-size: 24px;
      font-weight: 200;
      line-height: 150%;
      color: #000;
      margin-bottom: 32px;
    }

    .business-tags {
      font-size: 16px;
      font-weight: 400;
      line-height: 150%;
      color: #000;
    }

    .info-button {
      bottom: 0;
      // margin-bottom: 24px;
    }

    .business-img-box {
      position: absolute;
      right: 0;
      bottom: 0;
    }
  }
}

@media screen and (max-width: 599px) {
 
  .mobile_text{
    background-color: black;
    opacity: 0.7;
  }
  #business {
    background-color: #000;

    .business-title {
      font-size: 26px;
      font-weight: 500;
      line-height: 150%;
      color: #fff;
      margin-top: 300px;
      margin-bottom: 24px;
    }

    .business-desc {
      font-size: 18px;
      font-weight: 200;
      line-height: 150%;
      color: #fff;
      margin-bottom: 16px;
    }

    .business-tags {
      font-size: 14px;
      font-weight: 500;
      line-height: 150%;
      color: #fff;
    }

    .info-button {
      bottom: 0;
      // margin-bottom: 50px;
    }
  }
}

@media screen and (max-width: 599px) {
  #business {
    background-position: bottom, top, 0% 10%, center;
    background-size: cover;
  }
  .img-light {
    background-color: rgba(0, 0, 0, 0.4);
  }
}

@media screen and (max-width: 375px) {
  #business {
    background-color: #000;

    .business-title {
      font-size: 26px;
      font-weight: 500;
      line-height: 150%;
      color: #fff;
      margin-top: 150px;
      margin-bottom: 24px;
    }

    .business-desc {
      font-size: 18px;
      font-weight: 200;
      line-height: 150%;
      color: #fff;
      margin-bottom: 16px;
    }

    .business-tags {
      font-size: 14px;
      font-weight: 500;
      line-height: 150%;
      color: #fff;
    }

    .info-button {
      bottom: 0;
      margin-bottom: 12px;
    }
  }
}
</style>
