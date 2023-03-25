<template>
  <v-row class="mt-0">
    <v-carousel hide-delimiter-background height="70vh" progress="primary" show-arrows="hover" cycle>
      <v-carousel-item v-for="(slide, i) in slides" :key="i" :src="slide.src" cover class="align-center">
        <v-row no-gutters class="d-flex justify-start pa-16">
          <v-container>
            <v-sheet :width="450" :height="250" class="d-flex pa-4 align-center"
              style="background-color: rgb(43, 145, 42, 0.6); color: #fff;">
              <div class="text-h2 font-weight-black text-start">{{ slide.desc }}</div>
            </v-sheet>
          </v-container>
        </v-row>
      </v-carousel-item>
    </v-carousel>
  </v-row>
</template>

<script lang="ts">
import dam from '../assets/dam.jpeg';
import effluent from '../assets/effluent.webp';
import generator from '../assets/generator.webp';
import mine from '../assets/mine.jpeg';
import waste from '../assets/waste.jpeg';

export default {
  data() {
    return {
      slides: [
        {
          name: 'dam',
          src: dam,
          desc: 'Dam Construction',
        },
        {
          name: 'effluent',
          src: effluent,
          desc: 'Manufacturing Plants',
        },
        {
          name: 'generator',
          src: generator,
          desc: 'Heavy Duty Equipment',
        },
        {
          name: 'mine',
          src: mine,
          desc: 'Mining',
        },
        {
          name: 'waste',
          src: waste,
          desc: 'Waste Collection',
        },
      ],
    }
  },
}
</script>
