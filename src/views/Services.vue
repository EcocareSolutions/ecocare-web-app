<template>
  <v-container>
    <v-parallax height="40vh" src="@/assets/audit.png"
      class="mb-4 mt-16 text-center align-center justify-center d-flex">
      <v-sheet height="40vh" style="background: rgb(37,185,27);
            background: linear-gradient(90deg, rgba(37,185,27,1) 35%, rgba(255,255,255,0) 100%);" class="d-flex align-center">
        <v-container class="text-h3 font-weight-black d-flex align-center text-white">Our services include</v-container>
      </v-sheet>
    </v-parallax>
    <v-sheet class="mt-16">
      <v-slide-group v-model="model" class="pa-4" selected-class="bg-secondary" show-arrows>
        <v-slide-group-item v-for="n in services" :key="n" v-slot="{ toggle, selectedClass }">
          <v-card color="rgb(0, 87, 140, 0.5)" :class="['ma-4', selectedClass]" height="200" width="200" @click="toggle"
            elevation="4">
            <div class="d-flex text-h6 fill-height align-center text-white text-end justify-end pa-2 font-weight-black">
              {{ n }}
            </div>
          </v-card>
        </v-slide-group-item>
      </v-slide-group>

      <v-expand-transition>
        <v-sheet v-if="model != null" height="200">
          <div class="d-flex fill-height align-center justify-center">
            <h3 class="text-h6">
              Selected {{ model }}
            </h3>
          </div>
        </v-sheet>
      </v-expand-transition>
    </v-sheet>
    <v-sheet class="text-h6 font-weight-light pa-4 bg-secondary">
      Our Safety, Health and Environmental Impact Assessment Services
      Ecocare supports clients to undertake a number of projects from mining, cluster house building, fuel stations
      setting, water testing, environment management plans, safety and health.
    </v-sheet>

    <v-parallax height="40vh" src="@/assets/training.png"
      class="mb-4 mt-16 text-center align-center justify-center d-flex">
      <v-sheet height="40vh" style="background: rgb(37,185,27);
            background: linear-gradient(90deg, rgba(37,185,27,1) 35%, rgba(255,255,255,0) 100%);" class="d-flex align-center">
        <v-container class="text-h3 font-weight-black d-flex align-center text-white">Our training programs covers</v-container>
      </v-sheet>
    </v-parallax>
    <v-sheet>
      <v-slide-group v-model="model2" class="pa-4" selected-class="bg-primary" show-arrows>
        <v-slide-group-item v-for="n in thematic" :key="n" v-slot="{ toggle, selectedClass }">
          <v-card color="rgb(42, 143, 35, 0.6)" :class="['ma-4', selectedClass]" height="200" width="200" @click="toggle"
            elevation="4">
            <div class="d-flex text-h6 fill-height align-center text-white text-end justify-end pa-2 font-weight-black">
              {{ n }}
            </div>
          </v-card>
        </v-slide-group-item>
      </v-slide-group>

      <v-expand-transition>
        <v-sheet v-if="model2 != null" height="200">
          <div class="d-flex fill-height align-center justify-center">
            <h3 class="text-h6">
              Selected {{ model2 }}
            </h3>
          </div>
        </v-sheet>
      </v-expand-transition>
    </v-sheet>
    <v-sheet class="text-h6 font-weight-light pa-4 bg-primary mb-16">
      Capacity Development, Monitoring, and Evaluation Services Ecocare provides high-quality, customized
      capacity-building training that equips participants with the knowledge and skills they need to face day-to-day
      workplace and societal challenges with confidence.
    </v-sheet>

  </v-container>
</template>

<script lang="ts">
export default {
  data: () => ({
    model: null,
    model2: null,
    services: [
      'Prospectus reports',
      'Feasibility study',
      'Stake Emission Surveys',
      'Industrial Hygiene Surveys',
      'Environmental and Social Management Plans',
      'Environmental and Social Impact Assessment',
      'Environmental and Social Safeguards Assessments',
      'Environmental impact assessment final report',
      'Project costing',
      'Environmental quarterly reports',
      'Environmental audits',
      'Air emission surveys',
      'Waste disposal (expired drugs, expired medical utilities)'
    ],
    thematic: [
      'Institutional Capacity Development',
      'Environmental Social Safe Guards',
      'Project impact studies',
      'Project monitoring and evaluation studies',
      'Disaster Risk Reduction Management',
      'GIS and Mapping',
      'Baseline, Mid-term and Endline Surveys',
      'Third Party Monitoring Project Evaluation',
      'Water, Sanitation and Hygiene (WASH)',
      'Nutrition and Health development',
      'Food security and livelihoods',
      'Advocacy'
    ],
  }),
}
</script>
