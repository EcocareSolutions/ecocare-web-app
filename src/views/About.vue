<template>
  <div>
    <Carousel />
    <v-sheet height="30vh" style="
          background: rgb(37,185,27);
          background: linear-gradient(90deg, rgba(37,185,27,1) 55%, rgba(255,255,255,1) 100%);">
      <v-container class="text-h1 font-weight-black d-flex align-center text-white">About Us</v-container>
      <v-container class="text-h6 font-weight-light d-flex align-center text-white">Passionate about the
        environment</v-container>
    </v-sheet>
    <v-container>
      <v-row>
        <v-col cols="6"></v-col>
        <v-col cols="6" class="text-h6 font-weight-light">
          Ecocare aims to consistently provide a comprehensive range of high quality, professional and cost-effective
          services
          to our valued clientele, while promoting environmental best practices. Health and Safety, Wastewater treatment,
          Environmental impact assessment and Environmental Audit, Emissions Surveys is our area of expertise. Our
          business
          philosophy is guided and underpinned by the concept of sustainability, encompassing environmental, social and
          economic
          sustainability. Sustainability is a strategy for achieving economic and social development for all, whilst
          protecting
          the natural environment on which all life depends
        </v-col>
      </v-row>

      <v-row>
        <v-col cols="6" class="text-h6 font-weight-light">
          We registered in Zimbabwe since 2021, and with
          working experiences across Zimbabwe, ECOCARE strives towards providing and environmentally sustainable solutions
          and
          developing health and safety competencies within the public, private, and non- profit sectors. We do this
          through
          research, innovation, training, information dissemination, and quality technical assistance.
        </v-col>
        <v-col cols="6"></v-col>
      </v-row>
      <v-row>
        <v-col cols="6"></v-col>
        <v-col cols="6" class="text-h6 font-weight-light">
          At ECOCARE we recognize that change is the most constant element in today’s globalized and highly dynamic world.
          For individuals and institutions to be able to perform better at solving individual, organizational and societal
          challenges, ECOCARE believes that we must devise new, strategic, and creative ways of managing different
          divisions be it safety, health and environmental management, mining, energy, public management and monitoring and evaluation.
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="6" class="text-h6 font-weight-light">
          To achieve this, ECOCARE brings together a network of experienced professionals who have over 25 years of
          hands-on experience in the field of environmental management, safety and health, biotechnology, civil engineering,
          monitoring and evaluation, ecology, GIS, strategic management, project management and institutional capacity development
          and innovative technologies to develop efficient, effective, and practical solutions to everyday challenges at home,
          work and in our communities. ECOCARE has a robust national and international linkages with experts and organizations from across region. This
          allows us to tap into a wide range of experienced experts to undertake various consultancy assignments.
        </v-col>
        <v-col cols="6"></v-col>
      </v-row>
    </v-container>
  </div></template>

<script lang="ts" setup>
import Carousel from '@/components/Carousel.vue';
</script>
