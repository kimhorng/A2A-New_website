<<template>
  <section id="welcome" class="mt-12">
    <v-row>
      <v-container class="d-flex align-md-center">
        <v-col cols="12" sm="6" md="6" class="d-flex flex-column">
          <div id="welcome-container">
            <div
              class="display-1 mt-sm-12 mt-md-12 mb-6"
              style="color: #bd182a;"
              id="welcome-title"
            >
              <b> WE ARE HIRING!</b>
            </div>
            <div style="color: #bd182a;" id="mobile-title">
              <b> WE ARE HIRING!</b>
            </div>
            <v-img
              src="https://cdn.discordapp.com/attachments/668061712649420823/714895218046140446/welcome-page-vector-01.svg"
              alt="welcome-img"
              id="Mobile-img"
            ></v-img>
            <div class="welcome-text hidden-sm-and-down" v-text="welcome.text" />
            <div class="welcome-text hidden-md-and-up" v-text="welcome.text1" />
            <v-btn
              class="goto-careers d-flex align-center"
              to="/career"
              id="welcome-btn"
              outlined
              color="red darken-3"
            >
              <span>Go to Careers</span>
            </v-btn>
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
            src="https://cdn.discordapp.com/attachments/668061712649420823/714895218046140446/welcome-page-vector-01.svg"
            alt="welcome-img"
          ></v-img>
        </v-col>
      </v-container>
    </v-row>
    <v-row class="scroll_down_btn">
      <v-col cols="12" >
      <a >
        <div class="scroll_down mx-auto" @click="onScrolled">
          <v-col class="" style="margin-top:-20px;">
            <div class="chevron"></div>
            <div class="chevron"></div>
            <div class="chevron"></div>
          </v-col>
        </div>
      </a>
    </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      welcome: {
        text:
          'Join us on our journey to creating word-class experiences in Cambodia. At A2A, you will work in a vibrant, collaborative environment with smart, ambitious, motivated, well-rounded people from diverse cultures and of different nationalities, day-in and day-out.',
          text1:'Join us on our journey to creating word-class experiences in Cambodia. At A2A, you will work in a vibrant, collaborative environment with smart, ambitious, motivated.'
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
#welcome-btn{
  transition: 1s;
}
#welcome-btn:hover{
  margin-left: 10px;
}
#mobile-title {
  display: none;
}
#Mobile-img {
  display: none;
}
.scroll_down {
  // position: relative;
  color: #000;
  width: 50px;
  height: 50px;
  text-align: center;
}
.chevron {
  position: absolute;
  width: 28px;
  height: 8px;
  opacity: 0;
  transform: scale3d(0.5, 0.5, 0.5);
  animation: move 3s ease-out infinite;
}
.chevron:first-child {
  animation: move 3s ease-out 1s infinite;
}

.chevron:nth-child(2) {
  animation: move 3s ease-out 2s infinite;
}

.chevron:before,
.chevron:after {
  content: ' ';
  position: absolute;
  top: 0;
  height: 100%;
  width: 51%;
  background: grey;
}

.chevron:before {
  left: 0;
  transform: skew(0deg, 30deg);
}

.chevron:after {
  right: 0;
  width: 50%;
  transform: skew(0deg, -30deg);
}

@keyframes move {
  25% {
    opacity: 1;

  }
  33% {
    opacity: 1;
    transform: translateY(30px);
  }
  67% {
    opacity: 1;
    transform: translateY(40px);
  }
  100% {
    opacity: 0;
    transform: translateY(55px) scale3d(0.5, 0.5, 0.5);
  }
}


@media screen and (min-width: 960px) {
  .welcome-img {
    position: relative;
    top: -100px;
    max-width: 100%;
  }
  #welcome-container {
    position: relative;
  }
}

@media screen and (min-width: 600px) {
  #welcome {
    .container {

      .welcome-text {
        font-weight: 200;
        font-size: 20px;
        line-height: 150%;
        margin-bottom: 30px;
      }

      .goto-careers {
        width: 190px;
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
}
@media screen and (max-width: 1300px) {
  .welcome-img {
    top: -150px;
  }
}

@media screen and (max-width: 1100px) {
  #gif {
    left: 22%;
  }
  .welcome-img {
    top: -200px;
  }
}
@media screen and (max-width: 960px) {
  .welcome-img {
    top: -200px;
  }
}
@media screen and (max-width: 850px) {
  .welcome-img {
    top: -250px;
  }
}
@media screen and (max-width: 750px) {
  .welcome-img {
    width: 500px;
    top: -300px;
  }
}

@media screen and (max-width: 600px) {
  
  #Mobile-img {
    display: grid;
    width: 80%;
    margin-left: 5%;
    position: relative;
    top: -4%;
  }
  #welcome-container {
    position: relative;
    top: -15%;
  }
  .scroll_down_btn{
    margin-top: -25%;
  }
  .welcome-img {
    display: none;
  }

  #welcome {
    // padding-top: 56px;

    .container {
      // padding: 25px;

      .notice-box {
        margin-top: 36px;
        background-color: #bd182a;
        color: white;
        width: 144px;
        margin-bottom: 36px;
      }

      .welcome-text {
        position: relative;
        top: -5%;
        font-weight: 200;
        font-size: 16px;
        line-height: 150%;
        margin-bottom: 10px;
      }

      .goto-careers {
        width: 190px;
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

@media screen and (max-width: 441px) {
  .scroll_down_btn{
    margin-top: -30%;
  }
  #welcome-title {
    display: none;
  }
  #mobile-title {
    display: grid;
    margin-bottom: 20px;
    font-size: 25px;
    margin-top: 40px;
  }
  #welcome-btn {
    position: relative;
    top: -8%;
  }

  #welcome {
    padding-top: 20px;

    .container {
      // padding: 25px;

      .notice-box {
        margin-top: 36px;
        background-color: #bd182a;
        color: white;
        width: 144px;
        margin-bottom: 36px;
      }

      .welcome-text {
        font-weight: 200;
        font-size: 16px;
        line-height: 150%;
        margin-bottom: 36px;
      }

      .goto-careers {
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
  .scroll_down_btn{
    margin-top: -35%;
  }
  #welcome-title {
    display: none;
  }
  #mobile-title {
    display: grid;
    margin-bottom: 20px;
    font-size: 25px;
    margin-top: 40px;
  }
  #welcome-btn {
    position: relative;
    top: -8%;
  }

  #welcome {
    padding-top: 20px;

    .container {
      // padding: 25px;

      .notice-box {
        margin-top: 36px;
        background-color: #bd182a;
        color: white;
        width: 144px;
        margin-bottom: 36px;
      }

      .welcome-text {
        font-weight: 200;
        font-size: 16px;
        line-height: 150%;
        margin-bottom: 36px;
      }

      .goto-careers {
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
  .scroll_down_btn{
    margin-top: -45%;
  }
  #welcome-title {
    display: none;
  }
  #mobile-title {
    display: grid;
    margin-bottom: 15px;
    font-size: 25px;
    // margin-top: 5px;
  }
  #welcome-btn {
    position: relative;
    top: -8%;
  }

  #welcome {
    // padding-top: 20px;

    .container {
      // padding: 25px;

      .notice-box {
        margin-top: 36px;
        background-color: #bd182a;
        color: white;
        width: 144px;
        margin-bottom: 36px;
      }

      .welcome-text {
        font-weight: 200;
        font-size: 16px;
        line-height: 150%;
        margin-bottom: 36px;
      }

      .goto-careers {
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
