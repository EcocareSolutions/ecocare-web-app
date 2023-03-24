<template>
  <v-row no-gutters>
    <v-col cols="8" class="align-center justify-center" style="display: flex;">
      <v-container>
      <v-row class="text-center mb-16 align-center justify-center" style="display: flex;">
        <img src="@/assets/earth.webp" height="250" alt=""/>
      </v-row>

      <v-row class="text-h4 font-weight-light text-center">
          Help us preserve Earth for the next generation by getting EMA
          certified today!
      </v-row>
      </v-container>
    </v-col>
    <v-col cols="4" class="justify-end pr-7" style="display: flex;">
      <v-sheet height="70vh" :width="250" class="pa-4"
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
  data() {}
}
</script>
