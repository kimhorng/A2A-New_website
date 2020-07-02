<template>
  <div>
    <v-container>
      <v-col md="10" sm="12" class="mx-auto">
        <v-card class="mt-12" flat>
          <p class="mt-12 display-1" id="Title">
            Hospitality and Tourism Lecturer
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
              To serve as a lecturer in hospitality management courses in the
              Department of Tourism Management
            </li>
            <li>
              To conduct research and publish per the Department’s research
              themes and priority.
            </li>
            <li>
              To liaise with the Head of Tourism Management Program regarding
              students’ progress, attendance patterns and general adherence to
              the University’s Code of Conduct
            </li>
            <li>
              To mentor and advise students with any difficulties relating to
              subjects as required. Position Title Lecturer International
              Leaders in Tourism Management Reporting Line Head of Department
              Salary/Benefits 1,400$-1,600$ Location Kirirom Institute of
              Technology (Kirirom National Park) No. of Hiring 1 person Term
              Full Time Qualification Master Degree/PhD preferred
            </li>
            <li>
              To keep up to date professionally of current industry trends and
              relevant local industry in order to best prepare the students for
              their industry placement and future employment.
            </li>
            <li>
              To assist and participate in other School activities such as
              events, University’s Open Day, graduation, etc
            </li>
            <li>
              Assume various administrative tasks and responsibilities towards
              the Department and, as requested by the Head of Department
            </li>
            <li>
              Some weekends and evening duties may be required e.g. when there’s
              an event or open day or graduation preparation, student
              recruitment interview panels etc
            </li>
            <li>
              Other tasks that are assigned by the management
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
              At least a Master’s degree qualification (A PhD holder or close to
              completing a PhD degree is preferred) preferably in tourism
              management or related field
            </li>
            <li>
              At least 5 years experiences in teaching; a PhD holder is required
              to have one year experience (including teaching assistantship)
            </li>
            <li>
              Formal training in research methodology and track records in
              publications in the field of tourism and/or social sciences
            </li>
            <li>Project management skills and problem solving</li>
            <li>
              Proactive, flexible, creative, highly committed and willing to
              learn and grow
            </li>
            <li>
              Knowledge of international tourism and hospitality management
              industry
            </li>
            <li>
              Excellent in English communication skills both writing and
              speaking and problem solving
            </li>
            <li>Digital literacy in office packages</li>
            <li>Presentation skills and time management skills</li>
            <li>Must have excellent supervisory and leadership skills</li>
            <li>An analytical mind with strong math skills</li>
            <li>Good organizational and planning skills</li>
            <li>Reliable and trustworthy</li>
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
