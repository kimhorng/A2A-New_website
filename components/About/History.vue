<template>
  <div
    style="background-color: rgba(200, 200, 255, 0.7);"
    height="100%"
    flat
    id="H-Block"
  >
    <v-row
      id="H-Row"
      class="pb-12  hidden-sm-and-down"
      height="100%"
      style="overflow:hidden ;margin-right: 0px;margin-left: 0px;"
    >
      <v-col
        lg="3"
        md="12"
        sm="12"
        cols="12"
        class="ml-lg-12 ml-1 mb-sm-12 mt-10"
        id="H-Card"
      >
        <!-- History -->
        <v-card
          class=" ml-lg-10 mx-md-auto mx-sm-auto pb-4 pt-8 px-8 mx-auto"
          width="350px"
          flat
        >
          <p class=" headline text-center" id="Title">
            <b>A Brief History</b>
          </p>
          <p class="Content text-center">
            A2A Town (Cambodia) Co., Ltd. was established by Mr. Takeshi Izuka
            on 20th December 2011. As of 31st December 2018, the shared capital
            has increased to 12.2 Million USD and has a total of 386 employees
            from 8 different countries.
          </p>
        </v-card>
      </v-col>
      <v-col
        lg="8"
        md="12"
        sm="12"
        cols="12"
        class="ml-12 pl-12 pt-12 mt-md-12 mt-sm-12"
        style="overflow:hidden"
        id="Timeline"
      >
        <div class="mt-12 pt-12 mt-10 " flat>
          <ul class="progressbar pt-sm-12">
            <v-card height="3px" id="Line" flat width="100%"></v-card>
            <li>
              <div id="Upper2011" style="font-size: 16px;">
                <p class="">
                  Established A2A Town Co., Ltd. at Phnom Penh in Cambodia with
                  the capital 200, 000, 000 Riel (50,000 USD)
                </p>
                <div style="position:absolute; top:95%"><b>2011</b> <br /></div>
              </div>
            </li>
            <li>
              <div style="font-size: 16px; width:300px">
                <div class="my-5"><b>2013</b> <br /></div>
                <p>
                  Pre-Launch of vKirirom Pine Resort and Make a contract with
                  the Royal government of Cambodia regarding concession land for
                  the investment project to develop eco-tourism and the Started
                  vKirirom Nature Land Project.
                </p>
              </div>
            </li>
            <li>
              <div id="Upper2014" style="font-size: 16px;">
                <p>
                  Established "vKirirom Pte. Ltd." in Singapore and the
                  Pre-Launched of Kirirom Institute of Technology
                </p>
                <div style="position:absolute; top:95%"><b>2014</b> <br /></div>
              </div>
            </li>
            <li>
              <div style="font-size: 16px;">
                <div class="my-6"><b>2015</b> <br /></div>
                vKirirom Pine Resort Grand Opening
              </div>
            </li>
            <li>
              <div id="Upper2016" style="font-size: 16px;">
                Capital Increment of A2A Town (Cambodia) Co., Ltd to 8M USD

                <div class="my-2"><b>2016</b> <br /></div>
              </div>
            </li>
          </ul>
        </div>
      </v-col>
    </v-row>
    <div style="font-size: 16px;" id="T2018">
      <div class="mb-6"><b>2018</b> <br /></div>
      Launch of KIT dormitory owner's program and Launch of vKirirom
      International School (Primary School)
    </div>
    <div flat class="" id="V-Time">
      <v-timeline>
        <v-timeline-item
          v-for="n in History"
          :key="n"
          color="red darken-3"
          large
        >
          <template v-slot:opposite>
            <span class="white--text">{{ n.year }}</span>
          </template>
          <v-card
            class="elevation-2"
            style="background-corlor: white; opacity:0.7"
          >
            <div
              class="Content mx-auto text-center"
              style="width:90%; font-size:13px; line-height: 25px"
            >
              {{ n.event }}
            </div>
          </v-card>
        </v-timeline-item>
      </v-timeline>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    History: [
      {
        year: '2011',
        event:
          'Established A2A Town Co., Ltd. at Phnom Penh in Cambodia with the capital 200, 000, 000 Riel (50,000 USD)'
      },
      {
        year: '2013',
        event:
          'Pre-Launch of vKirirom Pine Resort and Make a contract with the Royal Government of Cambodia regarding concession land for the investment project to develop eco-tourism and the Started vKirirom Nature Land Project.'
      },
      {
        year: '2014',
        event:
          'Established "vKirirom Pte. Ltd." in Singapore and the Pre-Launched of Kirirom Institute of Technology (IT department)'
      },
      {
        year: '2015',
        event: 'vKirirom Pine Resort Grand Opening'
      },
      {
        year: '2016',
        event: 'Capital Increment of A2A Town (Cambodia) Co., Ltd to 8M USD'
      },
      {
        year: '2018',
        event:
          "Launch of KIT dormitory owners' program and Launch of vKirirom International School (Primary School)"
      }
    ]
  })
}
</script>
//
<style lang="scss" scoped>
// #H-Block {
//   height: 1000px;
// }
#H-Row {
  position: relative;
  padding-top: 20%;
}
#Line {
  background: #bd182a;
  color: rgba(248, 247, 216, 0.7);
}
#Upper2011,
#Upper2014 {
  position: relative;
  top: -300px;
}
#Upper2016 {
  position: relative;
  top: -225px;
}
#V-Time {
  display: none;
}
#T2018 {
  line-height: 35px;
  width: 200px;
  position: relative;
  top: -410px;
  left: 85%;
  #T-T {
    position: relative;
    left: -145px;
  }
}
.Content {
  font-size: 16px;
}
.progressbar {
  counter-reset: step;
  margin-top: 75px;
  padding: 0;

  li {
    list-style-type: none;
    float: left;
    width: 180px;
    position: relative;

    letter-spacing: 2px;
    &:before {
      content: counter(step);
      color: transparent;
      width: 20px;
      height: 20px;
      line-height: 50px;
      border: 3px solid #bd182a;
      display: block;
      position: absolute;
      margin-top: 10px;
      top: -12px;
      margin: 0 auto 10px auto;
      border-radius: 50%;
      background-color: #bd182a;
      letter-spacing: 0px;
    }
    &:after {
      content: '';
      position: absolute;
      width: 100%;
      height: 3px;
      background-color: red;
      top: 25px;
      left: -50%;
      z-index: -1;
    }
    &:first-child:after {
      content: none;
    }
    &.active {
      color: yellow;
      &:before {
        border-color: yellow;
      }
    }
    &.active + li:after {
      background-color: yellow;
    }
  }
}
@media only screen and (max-width: 1050px) {
  #Upper2011 {
    top: -270px;
  }
  #Upper2014 {
    top: -340px;
  }
  #Upper2016 {
    position: relative;
    top: -260px;
  }
  #T2018 {
    position: relative;
    top: -750px;
    left: 75%;
  }
  .progressbar {
    li {
      width: 160px;
    }
  }
}
@media only screen and (max-width: 1490px) {
  #Upper2014 {
    top: -300px;
  }
  #Upper2016 {
    top: -260px;
  }
  .progressbar {
    li {
      width: 160px;
    }
  }
  #T2018 {
    top: -405px;
    left: 80%;
  }
}
@media only screen and (max-width: 1390px) {
  #T2018 {
    left: 85%;
  }
}
@media only screen and (max-width: 1265px) {
  #Upper2014 {
    top: -310px;
  }
  #Upper2016 {
    top: -275px;
  }
  // #H-Block {
  //   height: 1600px;
  // }
  #T2018 {
    left: 750px;
    top: -410px;
  }
}
@media only screen and (max-width: 950px) {
  #T2018 {
    display: none;
  }
  .progressbar {
    li {
      width: 120px;
    }
  }
  #Upper {
    top: -320px;
  }
  #V-Time {
    display: grid;
  }
  #Timeline {
    display: none;
  }
}
@media only screen and (max-width: 650px) {
  // #H-Block {
  //   height: 2000px;
  // }
  #T2018 {
    display: none;
  }
  #V-Time {
    display: grid;
  }
  #Timeline {
    display: none;
  }
  #H-Card {
    overflow: scroll;
  }
}
@media only screen and (max-width: 450px) {
  // #H-Block {
  //   height: 2400px;
  // }
}
@media only screen and (max-width: 375px) {
  // #H-Block {
  //   height: 2700px;
  // }
}
@media only screen and (max-width: 325px) {
  // #H-Block {
  //   height: 3000px;
  // }
}
</style>
