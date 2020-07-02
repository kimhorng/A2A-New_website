<template>
  <div>
    <v-container>
      <v-col md="10" sm="12" class="mx-auto">
        <v-card class="mt-12" flat>
          <p class="display-1" id="Title">
            Head of Department of Tourism Management
          </p>
          <pre><p id="Content">FULL TIME,        KIT</p></pre>
        </v-card>
      </v-col>

      <!-- Responsibilities -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Responsibilties</h2>
          <ul class="pt-4" id="Content">
            <li>
              Coordinate all academic matters and activities at the department
              to meet with the objectives of KIT’s educational programs and
              long-term strategic plan
            </li>
            <li>
              Support and facilitate faculty recruitment, promotion, retention
              and professional development
            </li>
            <li>
              Develop strategies to increase student access, enrollment,
              retention, graduation and career-readiness
            </li>
            <li>
              Promote KIT’s partnerships with schools, universities, government
              institutes and the business sector
            </li>
            <li>
              Encourage and support research, grant-writing, publishing and
              other scholarly activities of the faculty
            </li>
            <li>
              Promote innovation and knowledge transfer between KIT and the
              private sector
            </li>
            <li>
              Coordinate accreditation efforts and the preparation of reports to
              various accrediting agencies
            </li>
            <li>
              Coordinate and work closely with the Vice President of Academic
              Affairs, Deans and the other Heads of Departments in cross-cutting
              areas including campus development, staff professional
              development, external relations, and source planning and
              allocation
            </li>
          </ul>
        </v-card>
      </v-col>

      <!-- Highly Preferred Qualifications -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Qualifications</h2>
          <ul class="pt-4">
            <li>
              MASTER’s degree in Tourism Management or related fields from an
              internationally accredited institution (PhD degree is preferable)
            </li>
            <li>
              A minimum of five years of full-time teaching experience in higher
              education institution
            </li>
            <li>
              Deep understanding of current issues in higher education,
              including governance and management, student affairs, digital
              education, faculty development, internationalization and
              industry-university partnerships
            </li>
            <li>
              Demonstrated experience in and commitment to working
              collaboratively with faculty members and academic staffs
            </li>
            <li>
              Ability to resolve conflicts and build consensus and effective
              internal and external relationship- building skills
            </li>
            <li>
              Experience fostering a climate of intellectual diversity, debate
              and inquiry among staffs and students
            </li>
            <li>
              Deep knowledge and understanding of local culture with
              international and global mindset and experience
            </li>
            <li>Excellent written and communication skills</li>
          </ul>
        </v-card>
      </v-col>

      <!-- Benefits -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Benefits and eligibility</h2>
          <ul class="pt-4">
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
