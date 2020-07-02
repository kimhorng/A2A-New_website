<template>
  <div>
    <v-container class="">
      <v-col md="10" sm="12" class="mx-auto">
        <v-card class="mt-12" flat>
          <p class="display-1" id="Title">
            Student Counsellor
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
              Conduct individual and group counseling sessions to advise and
              assist students with academics.
            </li>
            <li>
              Evaluate students’ attributes and assist them in realizing their
              objectives.
            </li>
            <li>
              Develop and implement counseling strategies with contemporary
              methods of mentoring.
            </li>
            <li>
              Identify behavioral problems and act appropriately to remedy the
              situation.
            </li>
            <li>
              Attention to societal and cultural differences in all student
              matters.
            </li>
            <li>
              Assess the development of students and highlight the sense of
              accomplishment.
            </li>
            <li>
              Complete evaluations, analyze results and provide purposeful
              feedback.
            </li>
            <li>
              Cooperate with parents, academic staff and external partners.
            </li>
            <li>Arrange and schedule orientation programs and internships.</li>
            <li>
              Advertise facilities and study programs to potential students
            </li>
            <li>
              Implement and facilitate educational and training workshops for
              academic staff
            </li>
            <li>Other tasks assigned by management.</li>
          </ul>
        </v-card>
      </v-col>

      <!-- Highly Preferred Qualifications -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Qualifications</h2>
          <ul class="pt-4">
            <li>
              Analytical thinker with strong problem-solving and
              conflict-resolution skills
            </li>
            <li>
              Excellent in English communication skills both writing and
              speaking and problem solving
            </li>
            <li>Presentation skills</li>
            <li>Time management skills</li>
            <li>Reliable and trustworthy</li>
            <li>
              Analytical thinker with strong problem-solving and
              conflict-resolution skills.
            </li>
            <li>Transparency judgment and attention in detail</li>
            <li>Good interpersonal, verbal and written communication skills</li>
            <li>Computer skills</li>
            <li>
              At least a Bachelor’s degree qualification (Master degree is
              preferred) preferably in education or related field
            </li>
            <li>
              At least 3 years experiences of related positions in academic
            </li>
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
