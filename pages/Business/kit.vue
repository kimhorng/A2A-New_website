<template>
  <div>
    <div class="hidden-xs-only">
      <section>
        <v-container>
          <v-row wrap class="mt-12 mb-12">
            <v-col cols="12" sm="6" md="6" class="my-auto">
              <p id="Title" class="headline">Kirirom Institute of Technology</p>
            </v-col>

            <v-col cols="12" sm="6" class="my-auto">
              <p id="Sub" class="pt-2">First boarding institute in Cambodia</p>
            </v-col>
          </v-row>
        </v-container>
      </section>

      <section>
        <v-row id="Background">
          <v-col class="bg" id="Img" alt="background"> </v-col>
        </v-row>
      </section>

      <section class="all_text" style="background-color: #fafafa">
        <v-container>
          <v-row wrap class="mx-auto">
            <v-col cols="10" class="pr-md-12 mx-auto" id="Text">
              <div class="mt-12 mb-12">
                <h2>
                  About KIT
                </h2>
                <p class="pt-4">
                  KIT was established in 2014 in Kirirom by Mr. Takeshi Izuka,
                  with a view to become a leading science and technology
                  university in Southeast Asia with excellent education,
                  cutting-edge research, and a commitment to green development
                  and a multicultural community. Presently, KIT consists of two
                  departments, Software Engineering and Tourism Management with
                  around 330 students from Cambodia and Japan. The
                  newly-established architecture department will begin accepting
                  students for the academic year 2020-21.
                </p>
                <p class="pt-4">
                  The institute provides a full sponsorship to all Cambodian
                  students, covering tuition fees, food, health insurance, and
                  dormitory. Through the sponsorship, students will have an
                  opportunity to live and work abroad after successfully
                  completing the 4-year program. To mention a few of KIT’s
                  achievements, both Batch 1 and Batch 2 students are 100%
                  placed and working in both Japanese and Cambodian Companies.
                  On an average, our students have a proven record of winning 4
                  to 5 competitions/ Hackathon/ Business Pitch every year. In
                  the near future, graduate and research programs will be
                  established and strengthened in order to promote R&D and
                  innovation at KIT.
                </p>
                <h2 class="pt-4">Vision</h2>
                <p class="pt-4">
                  A leading science and technology university in Southeast Asia
                  with an excellent education, cutting-edge research, and a
                  commitment to green development and a multicultural community.
                </p>
                <h2 class="pt-4">Mission</h2>
                <ul class="pt-4">
                  <li>
                    Provide life-changing academic and career opportunities for
                    all students, regardless of their family’s socio-economic
                    background
                  </li>
                  <li>
                    Foster innovation, creativity, and team spirit among
                    students
                  </li>
                  <li>
                    Establish a diverse and multicultural community conducive to
                    studying, living and workin
                  </li>
                  <li>
                    Produce young leaders with local and global understanding
                    and respect
                  </li>
                  <li>
                    Serve national and regional needs for digital workforce with
                    the fast-changing context of digital transformation and
                    industry 4.0
                  </li>
                </ul>
                <h2 class="mt-4 pt-4">Our values</h2>
                <ul class="pt-4">
                  <li>Respect</li>
                  <li>Professionalism</li>
                  <li>Excellence</li>
                  <li>Innovation and creativity</li>
                  <li>Independent thinking</li>
                </ul>
              </div>
            </v-col>
          </v-row>
          <v-card flat style="background-color: #fafafa" class="text-center">
            <h1 class="mb-12">Words from Alumni</h1>
            <v-img
              src="https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766618/News/pich-min_jmecn1_vjle3j.jpg"
            ></v-img>
            <v-row class="mx-auto">
              <v-col md="10" sm="12" class="mx-auto">
                <p class="pa-12">
                  "Through out these 4 years at KIT, I never imagined my today-self,
                  I have gain much experience not only in studying but life
                  experience. First year at KIT, I learnt a lot of fundamental of
                  programming and I adapted to environment at KIT really quick. I
                  got selected to join Sakura Winter Exchange program at Kyoto,
                  Japan when I was in second grade. KIT has a unique program for all
                  students called “Internship” which makes students grow faster by
                  themselves. Through out hard working, I received a great
                  opportunity to do internship in real working environment in Tokyo,
                  Japan during my third year of university. I was really grateful
                  and thankful to KIT. I believed everyone has the same opportunity
                  only it depends on how they reach and approach to the
                  opportunity."
                </p>
              </v-col>
            </v-row>
          </v-card>
        </v-container>
      </section>

      <!--  -->

      <section class="each_link">
        <v-row style="height: 100%">
          <v-flex class="my-auto">
            <div class="text-center">
              <a href="https://kit.edu.kh/" target="_blank" id="btn" style="text-decoration:none">
                <v-btn  width="150px" primary light outlined class="mx-auto secondary1--text text-capitalize">
                  <span class="title">Take a Tour</span>
                </v-btn>
              </a>
            </div>
          </v-flex>
        </v-row>
      </section>

      <section class="info pt-4">
        <v-container>
          <div class="text-center">
            <p> For more information,</p>
            <p>Visit our Facebook page: <a href="https://web.facebook.com/KITinstitute/?epa=SEARCH_BOX" target="_blanck" style="color: black">Kirirom Institute of Technology</a></p> 
            <p>Send us an email: register@kit.edu.kh</p> 
            <p>+855 (0)78 777 344</p>
          </div>  
        </v-container>  
      </section> 

      <section class="footer">
        <div class="img_responsive">
          <nuxt-link to="/business/property" class="link">
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
          <kit />
        </v-carousel-item>

        <v-carousel-item>
          <property />
        </v-carousel-item>

        <v-carousel-item>
          <vkirirom />
        </v-carousel-item>

        <v-carousel-item>
          <a2aDigital />
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
  }
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
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766595/A2A%20Image/a2a_construction-min_vcpdbc_k6j5sx.jpg');
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
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591030709/Homepage/kit_stu-min_lnu53h.jpg');
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
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1590766595/A2A%20Image/a2a_construction-min_vcpdbc_k6j5sx.jpg');
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
    background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591030709/Homepage/kit_stu-min_lnu53h.jpg');
    background-size: 100%, 100%, 100%, cover;
  }
}
</style>
