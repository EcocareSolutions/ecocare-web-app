<template>
  <v-row no-gutters>
    <v-col cols="8" class="align-center justify-center" style="display: flex;">
      <v-container>
        <v-parallax src="@/assets/research.jpeg" class="text-center mb-16 align-center justify-center d-flex">
          <div class="d-flex flex-column fill-height justify-center align-center text-white">

            <v-row class="text-h4 font-weight-black text-center">
              We action this through research, innovation, training, information
              dissemination, and quality technical assistance.
            </v-row>
          </div>
        </v-parallax>
      </v-container>
    </v-col>
    <v-col cols="4" class="justify-end pr-7" style="display: flex;">
      <v-sheet height="100vh" :width="250" class="pa-4"
        style="background-color: rgb(43, 145, 42); color: #fff; display: flex;">
        <div class="text-h4 font-weight-black text-center" style="align-self: center;">
          “We dont inherit the Earth from our ancestors, we borrow it
          from our children."
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
