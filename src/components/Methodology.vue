<template>
  <v-row no-gutters>
    <v-col cols="6" class="align-center justify-center" style="display: flex;">
      <v-parallax height="70vh" src="@/assets/research.jpeg" class="text-center align-center justify-center d-flex pa-4">
        <div class="d-flex flex-column fill-height justify-center align-center text-white">
          <v-row class="text-h4 font-weight-black text-center">
          Our business philosophy is guided and underpinned by the concept of sustainability, encompassing environmental,
          social and economic sustainability.
          </v-row>
        </div>
      </v-parallax>
    </v-col>
    <v-col cols="6" class="justify-end" style="display: flex;">
      <v-sheet height="70vh" class="pa-4 bg-primary" style="color: rgb(43, 145, 42); display: flex;">
        <div class="text-h4 font-weight-light text-start" style="align-self: center;">

          <div class="font-weight-black text-h2">About Us</div>
          Ecocare aims to consistently provide a comprehensive range of high quality, professional and cost-effective
          services to our valued clientele, while promoting environmental best practices. Health and Safety, Wastewater
          treatment, Environmental impact assessment and Environmental Audit, Emissions Surveys is our area of expertise.
        </div>
      </v-sheet>
    </v-col>
  </v-row>
</template>

<script lang="ts">
export default {
  data() { }
}
</script>
