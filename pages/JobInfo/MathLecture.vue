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
              Teaches courses in the discipline area of mathematics and
              statistics.
            </li>
            <li>
              Develops and designs curriculum plans to foster student learning,
              stimulate class discussions, and ensures student engagement.
            </li>
            <li>
              Provides tutoring and academic counseling to students, maintains
              classes related records, and assesses student coursework.
              Collaborates and supports colleagues regarding research interests
              and co-curricular activities.
            </li>
            <li>Typically reports to a department head</li>
            <li>
              Design and deliver teaching material across a range of modules or
              within a subject area
            </li>
            <li>
              Using appropriate teaching, learning support and assessment
              methods.
            </li>
            <li>
              Supervise student projects, field trips and, where appropriate,
              placements.
            </li>
            <li>
              Identify areas where current provision is in need of revision or
              improvement.
            </li>
            <li>
              Contribute to the planning, design and development of objectives
              and material.
            </li>
            <li>
              Set, mark and assess work and examinations and provide feedback to
              students.
            </li>
            <li>Develop research objectives, projects and proposals</li>
            <li>Conduct individual or collaborative research projects.</li>
            <li>
              Identify sources of funding and contribute to the process of
              securing funds. Write or contribute to publications or disseminate
              research findings using other appropriate media.
            </li>
            <li>
              Make presentations at conferences or exhibit work at other
              appropriate events
            </li>
          </ul>
        </v-card>
      </v-col>

      <!-- Highly Preferred Qualifications -->
      <v-col md="10" sm="12" class="mx-auto">
        <v-card flat>
          <h2>Qualifications</h2>
          <ul class="pt-4">
            <li>Knowledge Mathematic and statistics</li>
            <li>
              Excellent English communication skills both writing and speaking
              and problem solving
            </li>
            <li>Presentation skills</li>
            <li>Time management skills</li>
            <li>Must have excellent supervisory and leadership skills</li>
            <li>An analytical mind with strong math skills</li>
            <li>Good organizational and planning skills</li>
            <li>Reliable and trustworthy</li>
            <li>
              At least a Master’s degree qualification(A PhD or close to
              completing a PhD degree is preferred) preferably in Mathematics Or
              related field
            </li>
            <li>
              At least 5years experiences of related positions in teaching
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
