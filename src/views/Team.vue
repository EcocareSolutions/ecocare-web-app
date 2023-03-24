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

    <v-sheet class="text-h6 font-weight-black mt-4 pa-4 bg-secondary">
      To complete all of its assignments, Ecocare Solutions assembles a team of qualified and experienced researchers,
      trainers, and subject matter experts.
    </v-sheet>
  </v-container>
</template>

<script lang="ts">
export default {
  data: () => ({
    team: [
      {
        name: 'Theophilus',
        qualification: 'Masters Degrees in Monitoring and Evaluation and an executive certificates in program Monitoring and Evaluation',
        position: 'Monitoring and Evaluation',
      },
      {
        name: '',
        qualification: 'Masters Degrees in Monitoring and Evaluation and executive certificates in program Monitoring and Evaluation',
        position: 'Monitoring and Evaluation',
      },
      {
        name: '',
        qualification: 'PHD in Environmental Management',
        position: 'Environmental Management',
      },
      {
        name: '',
        qualification: 'Masters Degree in Public Health',
        position: 'Public Health',
      },
      {
        name: '',
        qualification: 'Master of Science degree in Sanitation and Wastewater Management',
        position: 'WASH',
      },
      {
        name: '',
        qualification: 'Degree in Biotechnology',
        position: 'Biotechnology',
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
