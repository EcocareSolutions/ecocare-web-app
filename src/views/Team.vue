<template>
  <v-container>
    <v-row>

      <v-card class="ma-4" width="344" v-for="player in team" :key="player.name">
        <v-img src="https://cdn.pixabay.com/photo/2016/08/08/09/17/avatar-1577909_1280.png" height="300" cover></v-img>

        <v-card-title>
          {{ player.name }}
        </v-card-title>

        <v-card-subtitle>
          {{ player.position }}
        </v-card-subtitle>

        <v-card-text>
          {{ player.qualification }}

        </v-card-text>
      </v-card>
    </v-row>
  </v-container>
  <v-sheet class="bg-primary">
    <v-container>
      <v-container class="text-h2 font-weight-black d-flex align-center text-white justify-center">Why Choose Ecocare
        Solutions</v-container>
      <v-container>
        <v-row no-gutters>
          <v-col cols="12" sm="4" class="d-flex align-center justify-center pa-8 text-h6 flex-column font-weight-light">
            <v-icon size="x-large" icon="mdi-cash-multiple"></v-icon>
            Value for Money
          </v-col>
          <v-col cols="12" sm="4" class="d-flex align-center justify-center pa-8 text-h6 flex-column font-weight-light">
            <v-icon size="x-large" icon="mdi-account-group"></v-icon>
            Customer Centric
          </v-col>
          <v-col cols="12" sm="4" class="d-flex align-center justify-center pa-8 text-h6 flex-column font-weight-light">
            <v-icon size="x-large" icon="mdi-shield-check"></v-icon>
            Integrity
          </v-col>
          <v-col cols="12" sm="4" class="d-flex align-center justify-center pa-8 text-h6 flex-column font-weight-light">
            <v-icon size="x-large" icon="mdi-hand-heart"></v-icon>
            Trust
          </v-col>
          <v-col cols="12" sm="4" class="d-flex align-center justify-center pa-8 text-h6 flex-column font-weight-light">
            <v-icon size="x-large" icon="mdi-head-heart"></v-icon>
            Fair
          </v-col>
          <v-col cols="12" sm="4" class="d-flex align-center justify-center pa-8 text-h6 flex-column font-weight-light">
            <v-icon size="x-large" icon="mdi-nature-people"></v-icon>
            Sustainable
          </v-col>
        </v-row>
      </v-container>
    </v-container>
  </v-sheet>
</template>

<script lang="ts">
export default {
  data: () => ({
    team: [
      {
        name: 'Theophilus',
        qualification: 'Masters Degrees in Monitoring and Evaluation and an executive certificates in program Monitoring and Evaluation',
        position: 'Team Leader',
      },
      {
        name: '',
        qualification: 'PHD in Environmental Management',
        position: 'Environmentalist',
      },
      {
        name: '',
        qualification: 'Masters Degree in Public Health',
        position: 'Social Scientist',
      },
      {
        name: '',
        qualification: 'Degree in Biotechnology',
        position: 'Biotechnician',
      },
      {
        name: '',
        qualification: 'Degree in Civil Engineering',
        position: 'Civil Engineer',
      },
      {
        name: '',
        qualification: 'Ecologist',
        position: 'Honors degree in Ecology',
      },
    ]
  })
}
</script>
