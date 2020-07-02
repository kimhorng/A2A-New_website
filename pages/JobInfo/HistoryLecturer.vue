<template>
  <div>
    <v-container class="">
      <v-col md="10" sm="12" class="mx-auto">
        <v-card class="mt-12" flat>
          <p class="display-1" id="Title">
            Khmer Culture and History Lecturer
          </p>
          <pre><p id="Content">PART TIME,        KIT</p></pre>
        </v-card>
      </v-col>

      <!-- Responsibilities -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Responsibilties</h2>
          <ul class="pt-4" id="Content">
            <li>
              Teach and educate students in the subject of Khmer Literature and
              History
            </li>
            <li>Control and follow up students’ discipline and behavior</li>
            <li>
              Prepare the lesson plan and update teaching materials and
              resources
            </li>
            <li>
              Strengthen and motivate students to study independently and
              cooperatively
            </li>
            <li>
              Teach students through the student center and new teaching methods
            </li>
            <li>Assess and evaluate students’ progress and behavior</li>
            <li>Conduct tests and ongoing assessments for students</li>
            <li>
              Join in the class council and cooperate with the teachers in
              charge
            </li>
            <li>Other tasks will assign by school management</li>
          </ul>
        </v-card>
      </v-col>

      <!-- Highly Preferred Qualifications -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Qualifications</h2>
          <ul class="pt-4">
            <li>Fully knowledge of Khmer history and international history</li>
            <li>Good of time management</li>
            <li>
              Good interpersonal skills, including cross cultural communication
            </li>
            <li>
              Must be able to prioritize work to meet scheduled deadlines while
              handling multiple tasks
            </li>
            <li>Very good in English communication skills</li>
            <li>Strong organizational and problem solving</li>
            <li>Master Degree in related field</li>
            <li>Hold a pedagogy training certificate</li>
            <li>At least 3year experiences teaching in higher education</li>
            <li>Computer Skills (Ms. Word & Excel and Internet and e-mail…)</li>
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
