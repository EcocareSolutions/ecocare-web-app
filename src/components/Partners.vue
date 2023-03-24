<template>
  <v-row no-gutters>
    <v-col cols="8" class="align-center justify-center" style="display: flex;">
      <v-container>
        <v-row class="text-center mb-4">
          <v-sheet elevation="2" class="ma-2 pa-2 align-center justify-center" style="display: flex;">
            <v-img src="@/assets/transparency.png" width="140" cover></v-img>
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
          <img src="@/assets/pigad.png" height="180" alt="" class="mt-2" />
          </v-sheet>
        </v-row>
        <v-row class="text-h4 font-weight-light text-center">
          We collaborate with public, private, and non-profit organizations. Transparency International, Oxfam, Danish
          church aid, ActionAid International, the government, Caritas, the European Mission in Zimbabwe, the
          Environmental Management Agency, PIGAD, and ZINWA are among the organizations involved.
        </v-row>
      </v-container>
    </v-col>
    <v-col cols="4" class="justify-end pr-7" style="display: flex;">
      <v-sheet :width="250" class="pa-4"
        style="background-color: rgb(43, 145, 42); color: #fff; display: flex;">
        <div class="text-h4 font-weight-black text-center" style="align-self: center;">
          "To go fast, go alone. To go far, go together!"
        </div>
      </v-sheet>
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
