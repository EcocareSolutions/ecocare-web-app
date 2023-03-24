<template>
    <v-row>
      <v-carousel hide-delimiter-background height="87vh" progress="primary" show-arrows="hover" cycle>
        <v-carousel-item v-for="(slide, i) in slides" :key="i" :src="slide.src" cover class="align-end">
          <v-row no-gutters>
            <v-col class="offset-8 justify-end pr-10" cols="4" style="display: flex;">
              <v-sheet height="90vh" :width="250" class="pa-4 align-center"
                style="background-color: rgb(43, 145, 42, 0.6); color: #fff; display: flex;">
                <div style="align-self: center;" class="text-h4 font-weight-black text-center">{{ slide.desc }}</div>
              </v-sheet>
            </v-col>
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
          desc: 'Do you have an EMA certification as you start building a dam on your farm?',
        },
        {
          name: 'effluent',
          src: effluent,
          desc: 'Where does the effluent from your industrial processes go to? Are you not contributing to water pollution?',
        },
        {
          name: 'generator',
          src: generator,
          desc: 'Did you know you need a certified EIA to assign a license to your generator if its rated 5Kva and above?',
        },
        {
          name: 'mine',
          src: mine,
          desc: 'Are you practicing eco-friendly mining yet have no certification to show compliance?',
        },
        {
          name: 'waste',
          src: waste,
          desc: 'ISO:9001 requires your organization to adhere to set waste management standards. Are you complying?',
        },
      ],
    }
  },
}
</script>
