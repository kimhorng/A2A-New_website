<template>
  <div>
    <v-row class="blue-grey lighten-5 pt-12" style="margin-left: 0px; margin-right:0px ">
      <v-col
        lg="12"
        md="12"
        sm="12"
        class="text-center display-1"
        style="margin-left: 0px; margin-right:0px "
      >
        Our Values
      </v-col>
    </v-row>
    <v-row class="blue-grey lighten-5 " style="margin-left: 0px; margin-right:0px ">
      <v-col lg="12" md="12" sm="12" cols="12">
        <!-- <v-container class="px-12"> -->
        <v-carousel
          :show-arrows="false"
          cycle="true"
          delimiter-icon="mdi-minus"
          hide-delimiter-background
          light
          height="200"
          class="center"
          style="margin-left: 0px; margin-right:0px "
        >
          <v-carousel-item class="text-center" style="margin-left: 0px; margin-right:0px ">
            <v-card flat class="transparent mt-6">
              <h1 class="display-1 black--text">Be Different</h1>
              <p class="grey--text">
                Respect, Professionalism, Excellence, Innovation and creativity
                , Independent thinking.
              </p>
            </v-card>
          </v-carousel-item>

          <v-carousel-item class="text-center" style="margin-left: 0px; margin-right:0px ">
            <v-card flat class="transparent mt-6">
              <h1 class="display-1 black--text">What can you find here?</h1>
              <p class="grey--text"
                >An Opportunites to work with Us
              </p>
            </v-card>
          </v-carousel-item>
        </v-carousel>
        <!-- </v-container> -->
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
