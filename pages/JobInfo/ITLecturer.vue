<template>
  <div>
    <v-container class="">
      <v-col md="10" sm="12" class="mx-auto">
        <v-card class="mt-12" flat>
          <p class="display-1" id="Title">
            Math Lecturer
          </p>
          <pre><p id="Content">FULL TIME,        KIT</p ></pre>
        </v-card>
      </v-col>

      <!-- Responsibilities -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Responsibilties</h2>
          <ul class="pt-4" id="Content">
            <li>
              Designs, develops, enhances, debugs, and implements software.
              Troubleshoots production problems related to software
              applications.
            </li>
            <li>
              Researches, tests, builds, and coordinates the conversion and/or
              integration of new products based on client requirements. Designs
              and develops new software products or major enhancements to
              existing software.
            </li>
            <li>
              Addresses problems of systems integration, compatibility, and
              multiple platforms
            </li>
            <li>
              Consult with project teams and end users to identify application
              requirements.
            </li>
            <li>
              Performs feasibility analysis on potential future projects to
              management
            </li>
            <li>
              Assists in the evaluation and recommendation of application
              software packages, application integration and testing tools.
            </li>
            <li>
              Resolves problems with software and responds to suggestions for
              improvements and enhancements.
            </li>
            <li>Acts as team leader on projects.</li>
            <li>
              Instructs, assigns, directs, and checks the work of other software
              developers on the development team.
            </li>
            <li>Participates in development of software user manuals.</li>
          </ul>
        </v-card>
      </v-col>

      <!-- Minimum Qualifications -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Minimum Qualifications</h2>
          <ul class="pt-4" id="Content">
            <li>
              Master degree in software engineering or relevant to information
              technology (or a Master’s degree with a minimum of four years’
              experience)
            </li>
            <li>
              More than 3 years of working experiences in teaching or software
              development project
            </li>
            <li>Project management skills and problem solving</li>
            <li>
              Proactive, flexible, creative, highly committed and willing to
              learn and grow
            </li>
          </ul>
        </v-card>
      </v-col>

      <!-- Highly Preferred Qualifications -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Highly Preferred Qualifications</h2>
          <ul class="pt-4">
            <li>
              Have involved in an actual product development and debugging
            </li>
            <li>Able to construct good relation with the students</li>
            <li>
              Have high adaptability and understanding to new and international
              environments
            </li>
          </ul>
        </v-card>
      </v-col>

      <!-- Benefits -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Benefits and eligibility</h2>
          <ul class="pt-4">
            <li>
              Working location is at Kirirom Institute of Technology, Kampong
              Speu province, Cambodia. Free returned shuttle bus services
              (KIT-Phnom Penh_KIT) for lecturers and students are available
              during the weekend
            </li>
            <li>
              Base salary of 1,200-1,500USD/month, depending on qualifications
              and experience
            </li>
            <li>Accident Insurance and health care on 24hrs</li>
            <li>Life insurance</li>
            <li>Yearly increment</li>
            <li>Severance paid and seniority payment</li>
            <li>Public holiday is followed Ministry of Labor</li>
            <li>Transportation</li>
            <li>Accommodation and 3time meals/day</li>
            <li>
              Others required by the labor law are complied with Cambodian labor
              law.
            </li>
          </ul>
        </v-card>
      </v-col>

      <v-col md="10" sm="12" class="mx-auto text-center">
        <v-btn
          class="my-6 "
          to="/applyform"
          outlined
          color="red darken-1"
          id="btn"
        >
          APPLY FOR THIS JOB
        </v-btn>
      </v-col>
    </v-container>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Footer from '../../layouts/Footer'
export default {
  components: {
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
</style>
