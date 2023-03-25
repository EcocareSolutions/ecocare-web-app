<template>
  <v-row no-gutters>
    <v-col cols="6" class="justify-end" style="display: flex;">
      <v-sheet class="pa-4" style="background-color: rgb(43, 145, 42); color: #fff; display: flex;">
        <div class="text-h4 font-weight-light text-end" style="align-self: center;">
          <div class="font-weight-black text-h2">Our Partners</div>
          We operate in distinguished market segments focusing on Infrastructure Development, Energy, Construction, Land
          Development, Water and Sanitation, Health and Safety, Manufacturing & Mining Industries
        </div>
      </v-sheet>
    </v-col>
    <v-col cols="6" class="align-center justify-space-between" style="display: flex;">
      <v-container class="pa-16">
        <v-row class="text-h4 font-weight-light text-center">
        </v-row>
        <v-row class="text-center align-center justify-center mb-4">
          <v-sheet elevation="2" class="ma-2 pa-2 align-center justify-center" style="display: flex;">
            <img src="@/assets/transparency.png" height="140" alt="" class="mt-2" />
          </v-sheet>
          <v-sheet elevation="2" class="ma-2 pa-2 align-center justify-center" style="display: flex;">
            <img src="@/assets/oxfam.jpeg" height="140" alt="" class="mt-2" />
          </v-sheet>
          <v-sheet elevation="2" class="ma-2 pa-2 align-center justify-center" style="display: flex;">
            <img src="@/assets/danish.png" height="140" alt="" class="mt-2" />
          </v-sheet>
          <v-sheet elevation="2" class="ma-2 pa-2 align-center justify-center" style="display: flex;">
            <img src="@/assets/goz.png" height="140" alt="" class="mt-2" />
          </v-sheet>
          <v-sheet elevation="2" class="ma-2 pa-2 align-center justify-center" style="display: flex;">
            <img src="@/assets/caritas.jpeg" height="140" alt="" class="mt-2" />
          </v-sheet>
          <v-sheet elevation="2" class="ma-2 pa-2 align-center justify-center" style="display: flex;">
            <img src="@/assets/ema.jpeg" height="140" alt="" class="mt-2" />
          </v-sheet>
          <v-sheet elevation="2" class="ma-2 pa-2 align-center justify-center" style="display: flex;">
            <img src="@/assets/zinwa.png" height="140" alt="" class="mt-2" />
          </v-sheet>
          <v-sheet elevation="2" class="ma-2 pa-2 align-center justify-center" style="display: flex;">
            <img src="@/assets/pigad.png" height="140" alt="" class="mt-2" />
          </v-sheet>
        </v-row>
      </v-container>
    </v-col>
  </v-row>
</template>

<script lang="ts">
export default {
  data() {
    return {
      partners: [
        "transparency.jpeg",
      ]
    }
  }
}
</script>
