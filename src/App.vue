<template>
  <v-app id="inspire">
    <v-app-bar height="85" flat>
      <v-container class="fill-height d-flex align-center">
        <v-avatar class="me-10 ms-4" size="60">
          <v-img contain height="300" src="@/assets/logo.jpeg" />
        </v-avatar>
        <div class="font-weight-black text-h4" style="color: #2B912A;">
          ECOCARE&nbsp;
        </div>
        <div class="font-weight-normal text-h4" style="color: #02578D;">
          SOLUTIONS
        </div>
        <v-spacer></v-spacer>

        <router-link v-for="link in links" :key="link.name" :to="link.href" style="text-decoration: none; color: black;">
          <v-btn variant="text" class="text-h5 font-weight-light">
            {{ link.name }}
          </v-btn>
        </router-link>

      </v-container>
    </v-app-bar>

    <v-main>
      <v-container style="padding-bottom: 0;">
        <v-row>
          <v-col>
            <v-sheet min-height="70vh" rounded="lg">
              <router-view />
            </v-sheet>
          </v-col>
        </v-row>
      </v-container>
    </v-main>

    <v-footer color="secondary">
      <v-container>
        <v-row no-gutters class="pa-8">
          <v-col cols="3">
            <v-row class="font-weight-black text-h5 mb-3">About</v-row>
            <v-row class="font-weight-light text-h6 mb-3">Our Story</v-row>
            <v-row class="font-weight-light text-h6 mb-3">Our Vision</v-row>
            <v-row class="font-weight-light text-h6 mb-3">Join the team</v-row>
          </v-col>
          <v-col cols="3">
            <v-row class="font-weight-black text-h5 mb-3">Customer Support</v-row>
            <v-row class="font-weight-light text-h6 mb-3">Customer Service</v-row>
            <v-row class="font-weight-light text-h6 mb-3">Contact Us</v-row>
            <v-row class="font-weight-light text-h6 mb-3">FAQs</v-row>
          </v-col>
          <v-col cols="3">
            <v-row class="font-weight-black text-h5 mb-3">Get Help</v-row>
            <v-row class="font-weight-light text-h6 mb-3">Live Chat</v-row>
            <v-row class="font-weight-light text-h6 mb-3">+263 78 992 7441</v-row>
            <v-row class="font-weight-light text-h6 mb-3">info@ecocaresolutions.co.zw</v-row>
          </v-col>
          <v-col cols="3">
            <v-row class="font-weight-black text-h5 mb-3">Connect With Us</v-row>
            <v-row class="justify-space-between">
              <v-icon icon="mdi-facebook"></v-icon>
              <v-icon icon="mdi-twitter"></v-icon>
              <v-icon icon="mdi-instagram"></v-icon>
              <v-icon icon="mdi-linkedin"></v-icon>
            </v-row>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script lang="ts">
export default {
  data: () => ({
    links: [
      {
        name: 'Home',
        href: 'home',
      },
      {
        name: 'About',
        href: 'about',
      },
      {
        name: 'Services',
        href: 'services',
      },
      {
        name: 'Team',
        href: 'team',
      },
      {
        name: 'Get In Touch',
        href: 'contact',
      },
    ],
  }),
}
</script>
