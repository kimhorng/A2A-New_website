<template>
  <div>
    <v-container class="">
      <v-card class="mt-12" flat>
        <v-card-title class="display-1" id="Title">
          Application Form
        </v-card-title>
        <v-card-subtitle id="Content">
          <pre><h3>FULL TIME,        PHNOM PENH</h3></pre>
        </v-card-subtitle>
      </v-card>
    </v-container>

    <!-- Application Form -->
    <div class="blue-grey lighten-5 mt-6 pt-6">
      <v-form method="post" action="#" v-model="isValid">
        <v-container>
          <v-col md="10" sm="12" class="mx-auto">
              <v-card flat>
                <div class="blue-grey lighten-5 ">
                  <v-card-text>
                    <b class="headline font-weight-regular"
                      >SUMMIT YOUR APPLICATION</b
                    >
                  </v-card-text>
                  <v-card-title>
                    Resume/CV
                  </v-card-title>
                  <v-card-subtitle>
                    Upload your resume in English (2 MB max). If the resume you
                    choose is a Google Drive file, we automatically create a copy.
                  </v-card-subtitle>

                  <v-card-action>
                    <div id="FileInput">
                      <v-btn
                        @click="onButtonClick"
                        class="ml-5 white"
                        text
                        color="red darken-1 "
                        outlined
                      >
                        <v-icon left>mdi-attachment</v-icon>
                        {{ buttonText }}
                      </v-btn>
                      <input
                        ref="uploader"
                        class="d-none"
                        type="file"
                        accept="image/*"
                        @change="onFileChanged"
                        required
                      />
                    </div>
                  </v-card-action>

                  <!-- Contact -->
                  <v-card-text>
                    <p class="title font-weight-regular">Contact details</p>
                  </v-card-text>
                  <div class="ml-5">
                    <v-row>
                      <v-col xl="12" lg="12" sm="12" md="12" cols="12">
                        <v-text-field
                          label="Name "
                          color="red darken-1"
                          v-model="name"
                          :rules="Rules"
                          required
                        />
                      </v-col>
                      <v-col xl="12" lg="12" sm="12" md="12" cols="12">
                        <v-select
                          color="red darken-1"
                          class="blue-grey lighten-5"
                          :items="Genders"
                          label="Gender"
                          v-model="gender"
                          :rules="Rules"
                          required
                        />
                      </v-col>
                    </v-row>

                    <v-text-field
                      label="Address "
                      color="red darken-1"
                      v-model="address"
                      :rules="Rules"
                      required
                    />
                    <v-text-field
                      label="Email "
                      color="red darken-1"
                      v-model="email"
                      :rules="emailRules"
                      required
                    />

                    <v-text-field
                      label="Phone Number "
                      color="red darken-1"
                      v-model="phoneNumber"
                      :rules="PhoneNumberRules"
                      required
                    />

                    <v-text-field
                      label="Nationality "
                      color="red darken-1"
                      v-model="nationality"
                      :rules="Rules"
                      required
                    />

                    <div class="mt-3">Marrital status:</div>
                    <v-radio-group
                      v-model="status"
                      :mandatory="false"
                      row
                      :rules="Rules"
                      required
                    >
                      <v-radio
                        label="Single"
                        value="single"
                        color="red darken-3"
                      ></v-radio>
                      <v-radio
                        label="Married"
                        value="married"
                        color="red darken-3"
                      ></v-radio>
                      <v-radio
                        label="Divorced"
                        value="divorced"
                        color="red darken-3"
                      ></v-radio>
                    </v-radio-group>
                  </div>

                  <!-- Degree -->
                  <v-card-text>
                    <p class="title font-weight-regular">Educational Background</p>
                  </v-card-text>
                  <!-- Display Degree Form -->
                  <div class="ml-5">
                    <v-text-field
                      label="School Name "
                      color="red darken-1"
                      v-model="schoolName"
                      :rules="Rules"
                      required
                    />

                    <v-text-field
                      label="Degree"
                      v-model="degree"
                      color="red darken-1"
                      :rules="Rules"
                      required
                    >
                    </v-text-field>

                    <v-text-field
                      label="Country/ Region"
                      color="red darken-1"
                      v-model="country"
                      :rules="Rules"
                      required
                    />

                    <v-text-field
                      label="Major"
                      v-model="major"
                      :rules="Rules"
                      required
                      color="red darken-1"
                    >
                    </v-text-field>
                    <hr class="red darken-1 my-6" v-if="i >= 2" />
                  </div>

                  <!-- Loop -->
                  <div class="ml-5" v-for="form in forms" :key="form">
                    <div>
                      Degree's Detail
                    </div>
                    <v-text-field
                      label="School Name "
                      color="red darken-1"
                      v-model="form.schoolName"
                    />

                    <v-text-field
                      label="Degree"
                      v-model="form.degree"
                      color="red darken-1"
                    >
                    </v-text-field>

                    <v-text-field
                      label="Country/ Region"
                      color="red darken-1"
                      v-model="form.country"
                    />

                    <v-text-field
                      label="Major"
                      v-model="form.major"
                      color="red darken-1"
                    >
                    </v-text-field>
                    <v-layout justify-end="">
                      <v-btn
                        v-on:click="
                          forms.splice(index, 1)
                          i--
                        "
                        class="red darken-1 white--text"
                      >
                        remove
                      </v-btn>
                    </v-layout>

                    <hr class="red darken-1 my-6" v-if="i >= 2" />
                  </div>

                  <v-btn
                    @click="AddDegreed()"
                    id="btn"
                    outlined
                    width="200px"
                    flat
                    class="subtitle-2  secondary1--text my-2 ml-5"
                  >
                    Add Another Degree
                  </v-btn>

                  <!-- Event -->
                  <v-card-text class="mt-6">
                    <p class="title font-weight-regular">
                      Trainings, volunteers, workshops
                    </p>
                  </v-card-text>
                  <!-- Display Event's card  -->
                  <div class="ml-5">
                    <div>Event's Detail</div>
                    <v-text-field
                      label="Event's Name/ Project"
                      color="red darken-1"
                      v-model="eventName"
                      :rules="Rules"
                      required
                    />
                    <v-text-field
                      label="Topic"
                      color="red darken-1"
                      v-model="topic"
                      :rules="Rules"
                      required
                    />
                    <v-text-field
                      label="Duration"
                      color="red darken-1"
                      v-model="duration"
                      :rules="Rules"
                      required
                    />
                    <v-text-field
                      label="Key Takeaway"
                      color="red darken-1"
                      v-model="key"
                      :rules="Rules"
                      required
                    />
                    <hr class="red darken-1 my-6" v-if="j >= 2" />
                  </div>

                  <!-- Loop -->
                  <div class="ml-5" v-for="event in events" :key="event">
                    <div>
                      Event's Detail
                    </div>
                    <v-text-field
                      label="Event's Name/ Project"
                      color="red darken-1"
                      v-model="event.eventName"
                    />
                    <v-text-field
                      label="Topic"
                      color="red darken-1"
                      v-model="event.topic"
                    />
                    <v-text-field
                      label="Duration"
                      color="red darken-1"
                      v-model="event.duration"
                    />
                    <v-text-field
                      label="Key Takeaway"
                      color="red darken-1"
                      v-model="event.key"
                    />
                    <v-layout justify-end="">
                      <v-btn
                        v-on:click="
                          events.splice(index, 1)
                          j--
                        "
                        class="red darken-1 white--text"
                      >
                        remove
                      </v-btn>
                    </v-layout>
                    <hr class="red darken-1 my-6" v-if="j >= 2" />
                  </div>

                  <v-btn
                    @click="AddEvent"
                    outlined
                    width="200px"
                    flat
                    class="subtitle-2  secondary1--text my-2 ml-5"
                  >
                    Add Another Event
                  </v-btn>

                  <!-- Work Exp -->
                  <v-card-text class="mt-6">
                    <p class="title font-weight-regular">Work experience</p>
                  </v-card-text>
                  <h5 class="ml-4">
                    Applying for the first job?
                  </h5>
                  <v-radio-group
                    v-model="FirstJob"
                    :rules="Rules"
                    required
                    row
                    class="ml-4"
                  >
                    <v-radio label="Yes" value="yes" color="red"></v-radio>
                    <v-radio label="No" value="no" color="red"></v-radio>
                  </v-radio-group>
                  <!-- Display Current Job's Form -->
                  <div v-show="FirstJob == 'no'" class="ml-5">
                    <div>Employee's Detail</div>
                    <v-text-field
                      label="Company name"
                      color="red darken-1"
                      v-model="company"
                    />

                    <v-text-field
                      label="Type of business"
                      color="red darken-1"
                      v-model="business"
                    />

                    <v-text-field
                      label="Job title"
                      color="red darken-1"
                      v-model="title"
                    />

                    <!-- Start Date -->
                    <div class="grey--text">Start date</div>
                    <v-row>
                      <v-col xl="6" lg="6" sm="6" md="6" cols="12">
                        <v-select
                          :items="Months"
                          label="Month"
                          v-model="StartMonth"
                          color="red darken-1"
                        />
                      </v-col>
                      <v-col xl="6" lg="6" sm="6" md="6" cols="12">
                        <v-text-field
                          label="Year (yyyy)"
                          color="red darken-1"
                          v-model="StartYear"
                        />
                      </v-col>
                    </v-row>
                    <v-text-field
                      label="Reason for leaving"
                      color="red darken-1"
                      v-model="leavingReason"
                    />

                    <!-- Current Job -->
                    <h5>
                      Is this your current job?
                    </h5>
                    <v-radio-group v-model="CurrentJob" row>
                      <v-radio label="Yes" value="yes" color="red"></v-radio>
                      <v-radio label="No" value="no" color="red"></v-radio>
                    </v-radio-group>

                    <!-- End Date -->
                    <div v-show="CurrentJob == 'no'">
                      <div class="grey--text">End Date</div>
                      <v-row>
                        <v-col xl="6" lg="6" sm="6" md="6" cols="12">
                          <v-select
                            :items="Months"
                            label="Month"
                            v-model="EndMonth"
                            color="red darken-1"
                          />
                        </v-col>
                        <v-col xl="6" lg="6" sm="6" md="6" cols="12">
                          <v-text-field
                            label="Year (yyyy)"
                            color="red darken-1"
                            v-model="EndYear"
                          />
                        </v-col>
                      </v-row>
                    </div>
                    <hr class="red darken-1 my-6" v-if="k >= 2" />
                  </div>

                  <!-- Current/ Recently Job's Form : LOOP -->
                  <div
                    v-show="FirstJob == 'no'"
                    class="ml-5"
                    v-for="job in jobs"
                    :key="job"
                  >
                    <div>
                      Employee's Detail
                    </div>
                    <v-text-field
                      label="Company name"
                      color="red darken-1"
                      v-model="job.company"
                    />

                    <v-text-field
                      label="Type of business"
                      color="red darken-1"
                      v-model="job.business"
                    />

                    <v-text-field
                      label="Job title"
                      color="red darken-1"
                      v-model="job.title"
                    />

                    <!-- Start Date -->
                    <div class="grey--text">Start date</div>
                    <v-row>
                      <v-col xl="6" lg="6" sm="6" md="6" cols="12">
                        <v-select
                          :items="Months"
                          label="Month"
                          v-model="job.StartMonth"
                          color="red darken-1"
                        />
                      </v-col>
                      <v-col xl="6" lg="6" sm="6" md="6" cols="12">
                        <v-text-field
                          label="Year (yyyy)"
                          color="red darken-1"
                          v-model="job.StartYear"
                        />
                      </v-col>
                    </v-row>
                    <v-text-field
                      label="Reason for leaving"
                      color="red darken-1"
                      v-model="job.leavingReason"
                    />

                    <!-- Current Job -->
                    <h5>
                      Is this your current job?
                    </h5>
                    <v-radio-group v-model="CurrentJob" row>
                      <v-radio label="Yes" value="yes" color="green"></v-radio>
                      <v-radio label="No" value="no" color="red"></v-radio>
                    </v-radio-group>

                    <!-- End Date -->
                    <div v-show="CurrentJob == 'no'">
                      <div class="grey--text">End Date</div>
                      <v-row>
                        <v-col xl="6" lg="6" sm="6" md="6" cols="12">
                          <v-select
                            :items="Months"
                            label="Month"
                            v-model="job.EndMonth"
                            color="red darken-1"
                          />
                        </v-col>
                        <v-col xl="6" lg="6" sm="6" md="6" cols="12">
                          <v-text-field
                            label="Year (yyyy)"
                            color="red darken-1"
                            v-model="job.EndYear"
                          />
                        </v-col>
                      </v-row>
                    </div>
                    <v-layout justify-end="">
                      <v-btn
                        v-on:click="
                          jobs.splice(index, 1)
                          k--
                        "
                        class="red darken-1 white--text"
                      >
                        remove
                      </v-btn>
                    </v-layout>
                    <hr class="red darken-1 my-6" v-if="k >= 2" />
                  </div>
                  <v-btn
                    class="red--text my-2"
                    id="btn"
                    @click="AddJob"
                    v-show="FirstJob == 'no'"
                    text
                  >
                    Add another job
                  </v-btn>
                  <!-- End  -->

                  <!-- Language -->
                  <v-card-text class="mt-6">
                    <p class="title font-weight-regular">Language(s)</p>
                  </v-card-text>
                  <v-card-action>
                    <v-card width="515" class="blue-grey lighten-5" flat>
                      <v-layout>
                        <v-card-text>
                          <b> Khmer</b>
                        </v-card-text>
                        <v-rating
                          v-model="khmer"
                          :rules="Rules"
                          required
                          background-color="red lighten-3"
                          color="red"
                          class="mt-1"
                        ></v-rating>
                      </v-layout>

                      <v-layout>
                        <v-card-text>
                          <b>English</b>
                        </v-card-text>
                        <v-rating
                          v-model="english"
                          :rules="Rules"
                          required
                          background-color="red lighten-3"
                          color="red"
                          class="mt-1"
                        ></v-rating>
                      </v-layout>
                    </v-card>
                    <ul style="position:relative;left:-9px">
                      <li
                        is="todo-item"
                        v-for="(todo, index) in todos"
                        v-bind:key="todo.id"
                        v-bind:title="todo.title"
                        v-on:remove="todos.splice(index, 1)"
                      >
                        <v-card flat width="500" class="blue-grey lighten-5 ">
                          <v-layout>
                            <div class="mt-1">
                              <b> {{ todo.language }}</b>
                            </div>
                            <v-spacer></v-spacer>
                            <v-rating
                              v-model="todo.rating"
                              :rules="Rules"
                              required
                              background-color="red lighten-3"
                              color="red"
                              class="mt-1"
                            ></v-rating>
                          </v-layout>
                          <v-layout justify-end="">
                            <v-btn
                              v-on:click="todos.splice(index, 1)"
                              id="btn1"
                              outlined
                              width="100px"
                              flat
                              class="subtitle-2  secondary1--text mt-9 ml-12"
                              >Remove</v-btn
                            >
                          </v-layout>
                        </v-card>
                      </li>
                    </ul>
                  </v-card-action>
                  <!-- Testing -->
                  <div id="todo-list-example" class="ml-4">
                    <form v-on:submit.prevent="addNewTodo">
                      <label for="new-todo" style="color:#C62828"
                        ><b><u>Add new Langauge?</u></b></label
                      >
                      <v-text-field
                        v-model="newTodoText"
                        id="new-todo"
                        label="Exampl: Thai, Japanese"
                        color="red darken-1"
                      />
                      <button :disabled="newTodoText.length == 0" id="addBtn">
                        Add
                      </button>
                    </form>
                  </div>

                  <!-- Optional Question -->
                  <v-card-text class="mt-6">
                    <p class="title font-weight-regular">Computer skills</p>
                  </v-card-text>
                  <div>
                    <v-text-field
                      label="Example: Microsoft office, Internet, Email, etc"
                      color="red darken-1"
                      v-model="skill"
                      :rules="Rules"
                      required
                      class="my-4 ml-5"
                    />
                  </div>
                  <v-card-text>
                    <p class="title font-weight-regular">
                      Why do you want to join us?
                    </p>
                  </v-card-text>
                  <div>
                    <v-text-field
                      label="Write your optional cover letter here"
                      color="red darken-1"
                      v-model="Q1"
                      class="my-4 ml-5"
                      :rules="Rules"
                      required
                    />
                  </div>
                  <v-card-text>
                    <p class="title font-weight-regular">How did you hear me?</p>
                  </v-card-text>
                  <div class="ml-5">
                    <div>
                      <v-text-field
                        label="Write your optional cover letter here"
                        color="red darken-1"
                        v-model="Q2"
                        class="my-4"
                        :rules="Rules"
                        required
                      />
                    </div>

                    <v-dialog v-model="dialog" persistent max-width="500">
                      <template v-slot:activator="{ on }">
                        <v-card
                          flat
                          width="80"
                          class="mt-6 mb-6 blue-grey lighten-5"
                          id="B-Card"
                        >
                          <v-btn
                            outlined
                            width="100px"
                            flat
                            class="subtitle-2 learnmore secondary1--text"
                            v-on="on"
                            :disabled="!isValid"
                          >
                            submit
                          </v-btn>
                        </v-card>
                      </template>
                      <v-card flat id="SubmitBox">
                        <v-card class="teal accent-3" height="50%" flat>
                          <v-icon color="white" size="100" class="Check"
                            >mdi-check-circle-outline</v-icon
                          >
                        </v-card>
                        <v-card
                          flat
                          max-height="50%"
                          class="text-center pt-6"
                          color="blue-grey--text darken-4"
                        >
                          <div class="display-1 mb-3">Great!</div>
                          <div class="mb-8">
                            Your information has submitted successfully.
                          </div>
                          <v-btn class="amber white--text" text to="/">
                            Start Exploring
                            <v-icon class="ml-2"> mdi-arrow-right</v-icon>
                          </v-btn>
                        </v-card>
                      </v-card>
                    </v-dialog>
                  </div>
                </div>
              </v-card>
          </v-col>
        </v-container>
      </v-form>
    </div>

    <footer>
      <Footer />
    </footer>
  </div>
</template>
<script>
import File from '../components/Form/File'
import Footer from '../layouts/Footer'
export default {
  data: () => ({
    // Single Variables
    isValid: false,
    add: false,
    hasHr: false,
    snackbar: false,

    name: '',
    gender: '',
    address: '',
    email: '',
    status: '',
    i: 1,
    j: 1,
    k: 1,
    phoneNumber: '',
    nationality: '',
    FirstJob: '',
    CurrentJob: '',
    khmer: '',
    english: '',
    skill: '',
    Q1: '',
    Q2: '',
    // Testing
    isDis: true,
    newTodoText: '',
    newRating: 0,
    todos: [],
    nextTodoId: 4,
    //  Rule
    Rules: [v => !!v || 'required!'],
    PhoneNumberRules: [
      v => !!v || 'Phone Number is required!',
      v => /\d/.test(v) || 'Number only!',
      v =>
        /^\+(?:[0-9] ?){6,14}[0-9]$/ ||
        "That's a Phone Number, They must be 9 or 10 digits. Example: xxx xxx xxx"
    ],
    emailRules: [
      v => !!v || 'Email is required',
      v =>
        /.+@.+/.test(v) || 'E-mail must be valid, Example: username@gmail.com'
    ],
    YearRules: [
      v => /\d/.test(v) || 'Number only!',
      v => !!v || 'Year is required'
    ],
    // Objects
    Genders: ['Male', 'Female', 'Other'],
    Months: [
      'January',
      'Februrary',
      'March',
      'April',
      'May',
      'June',
      'July',
      'August',
      'September',
      'October',
      'November',
      'December'
    ],
    Languages: ['Japanese', 'Chinese', 'France', 'Indian'],
    forms: [],
    events: [],
    jobs: [],
    languages: [],
    defaultButtonText: 'ATTACH RESUME/CV',
    selectedFile: null,
    isSelecting: false
  }),
  components: {
    File,
    Footer
  },
  computed: {
    buttonText() {
      return this.selectedFile ? this.selectedFile.name : this.defaultButtonText
    }
  },
  methods: {
    // Testing
    addNewTodo: function() {
      this.todos.push({
        id: this.nextTodoId++,
        language: this.newTodoText,
        rating: this.newRating
      })
      this.newTodoText = ''
    },
    onButtonClick() {
      this.isSelecting = true
      window.addEventListener(
        'focus',
        () => {
          this.isSelecting = false
        },
        { once: true }
      )

      this.$refs.uploader.click()
    },
    onFileChanged(e) {
      this.selectedFile = e.target.files[0]

      // do something
    },
    AddDegreed() {
      this.i += 1
      if (this.i > 1) {
        this.hasHr = true
      }
      this.forms.push({
        schoolName: '',
        degree: '',
        country: '',
        major: ''
      })
    },
    AddEvent() {
      this.j += 1
      this.events.push({
        eventName: '',
        topic: '',
        duration: '',
        key: ''
      })
    },
    AddJob() {
      this.k += 1
      this.jobs.push({
        company: '',
        business: '',
        title: '',
        StartMonth: '',
        StartYear: '',
        leavingReason: '',
        EndMonth: '',
        EndYear: ''
      })
    },
    AddLanguage() {
      this.add = !this.add
      this.languages.push({
        language: '',
        rating: ''
      })
    }
  }
}
</script>
<style lang="scss" scoped>
#addBtn {
  position: relative;

  color: #e53935;
  border: 1px solid #e53935;
  padding-left: 6px;
  padding-right: 6px;
  border-radius: 10px;
}
#SubmitBox {
  height: 400px;
}
#FileInput {
  overflow: scroll;
}
.Check {
  top: 25%;
  left: 40%;
}
@media screen and (max-width: 600px) {
  .Check {
    left: 35%;
  }
}
#btn {
  transition: 0.5s;
}
#btn:hover {
  font-size: 15px;
}
@media screen and (max-width: 600px) {
  #SubmitBox {
    height: 450px;
  }
}
</style>
