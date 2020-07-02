<template>
  <div>
    <v-container class="">
      <v-col md="10" sm="12" class="mx-auto">
        <v-card class="mt-12" flat>
          <p class="display-1" id="Title">
            Facilities Manager
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
              Day to day operate on campus by overseeing all aspects of facility
              maintenance, school safety health and cleanliness
            </li>
            <li>
              Daily monitor of the security personal at the school and student
              dormitory to ensuring all procedures are adhered to and
              time-keeping of their schedules
            </li>
            <li>
              Ability to withstand a variety of indoor and outdoor environmental
              conditions
            </li>
            <li>
              Inspect school facilities for the purpose of ensuring that all
              facilities are suitable for safe operations, and maintained in an
              attractive and cleaning
            </li>
            <li>
              Perform cleaning and special custodial work as required. Plan,
              schedule, and perform preventative
            </li>
            <li>
              Maintain knowledge regarding methods of cleaning, safety practices
              and procedures, and health standards
            </li>
            <li>
              Organize the set up and take down of equipment required by the
              school during school or after school activities
            </li>
            <li>
              Ensure security personally have the correct concerned ministry
              documentation in place
            </li>
            <li>
              Daily and monthly bus arrangement for student/staff and lecturer
            </li>
            <li>Ensure an equal distribution of classroom furniture</li>
            <li>
              Cooperate with resort team to prepare accommodation and food
              school events
            </li>
            <li>Other tasks assigned by management.</li>
          </ul>
        </v-card>
      </v-col>

      <!-- Highly Preferred Qualifications -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Highly referred Qualifications</h2>

          <ul class="pt-4">
            <li>Reliable and trustworthy</li>
            <li>
              Analytical thinker with strong problem-solving skills
            </li>
            <li>Transparency judgment and attention in detail</li>
            <li>Detail-oriented with excellent time-management skills</li>
            <li>Good interpersonal, verbal and written communication skills</li>
            <li>Computer skills</li>
            <li>
              At least a Bachelor’s degree qualification (Master degree is
              preferred) or related field
            </li>
            <li>
              At least 3 years experience in related positions in the education
              sector.
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
