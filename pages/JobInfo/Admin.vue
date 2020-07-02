<template>
  <div>
    <v-container class="">
      <v-col md="10" sm="12" class="mx-auto">
        <v-card class="mt-12" flat>
          <p class="display-1" id="Title">
            HR and Admin Officer
          </p>
          <pre><p id="Content">FULL TIME,        KIT</p></pre>
        </v-card>
      </v-col>

      <!-- Responsibilities -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Responsibilties</h2>
          <ul id="Content" class="pt-4">
            <li>
              Provides of administration for all functions in the School,
              including administration assistance and academic related
              administration activities
            </li>
            <li>
              Investigate and understand causes for staff and lecturer absences
            </li>
            <li>
              Daily checking and monthly attendance for staff and lecturer
            </li>
            <li>Stationery control</li>
            <li>
              Provide administrative assistance regarding HR and Admin-related
              activities such as recruitment requests and staff work
              plans/roster, follow up all expatriate staff of visa extension
            </li>
            <li>
              Travel arrangements: organize all work travel arrangements for
              staff/student within the school.
            </li>
            <li>Ensure the shuttle bus usage is fit to the business purpose</li>
            <li>
              Prepare all kinds of requests when the school needs any supply
            </li>
            <li>Make student’s ID card, Support student insurance</li>
            <li>
              Support for arranging examinations and assisting lecturer for
              examination
            </li>
            <li>
              Supports teachers to collect all exam papers for registrar’s
              department
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
            <li>Knowledge of general office practices and procedures</li>
            <li>Good of time management</li>
            <li>
              Must be able to prioritize work to meet scheduled deadlines while
              handling multiple tasks
            </li>
            <li>Good in English communication skills</li>
            <li>Strong organization and problem solving</li>
            <li>
              Bachelor Degree in related field and welcome for fresh graduate
              student
            </li>
            <li>At least 1year experience related</li>
            <li>
              Preferred candidate who are experiences in education industrial
            </li>
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
