<template>
  <v-container>
    <v-container class="text-h3 font-weight-black d-flex align-center text-primary">We would love to hear from you</v-container>
    <v-row>
      <v-col cols="6" class="d-flex flex-column mt-16">
      <div class="text-h5 font-weight-light d-flex align-center">Visit Us</div>
      <v-container class="d-flex flex-column">
      <div>64 Jengwa Street</div>
      <div>Madokero</div>
      <div>Harare</div>
      <div>Zimbabwe</div>
      </v-container>
      <div class="text-h5 font-weight-light d-flex align-center">Call Us</div>
      <v-container class="d-flex flex-column">
      <div>+263 773 243 234</div>
      <div>+263 719 343 434</div>
      </v-container>
      <div class="text-h5 font-weight-light d-flex align-center mb-4">Like our pages</div>
      <v-container class="justify-start">
              <v-icon icon="mdi-facebook" size="x-large" class="mr-4"></v-icon>
              <v-icon icon="mdi-twitter" size="x-large" class="mr-4"></v-icon>
              <v-icon icon="mdi-instagram" size="x-large" class="mr-4"></v-icon>
              <v-icon icon="mdi-linkedin" size="x-large" class="mr-4"></v-icon>
            </v-container>
      </v-col>
      <v-col cols="6" class="mt-16">
    <div class="text-h5 font-weight-light d-flex align-center">Send us a message</div>
        <form>
          <v-text-field v-model="state.name" :error-messages="v$.name.$errors.map(e => e.$message)" :counter="10"
            label="Name" required @input="v$.name.$touch" @blur="v$.name.$touch"></v-text-field>

          <v-text-field v-model="state.email" :error-messages="v$.email.$errors.map(e => e.$message)" label="E-mail"
            required @input="v$.email.$touch" @blur="v$.email.$touch"></v-text-field>

          <v-text-field v-model="state.message" :error-messages="v$.message.$errors.map(e => e.$message)" label="Message"
            required @input="v$.message.$touch" @blur="v$.message.$touch"></v-text-field>

          <v-btn class="me-4" @click="v$.$validate">
            submit
          </v-btn>
          <v-btn @click="clear">
            clear
          </v-btn>
        </form>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import { reactive, ref } from 'vue'
import { useVuelidate } from '@vuelidate/core'
import { email, required } from '@vuelidate/validators'

export default {
  setup() {
    const initialState = {
      name: '',
      email: '',
      message: '',
      select: null,
    }

    const state = reactive({
      ...initialState,
    })

    const rules = {
      name: { required },
      email: { required, email },
      message: { required },
    }

    const v$ = useVuelidate(rules, state)

    function clear() {
      v$.value.$reset()

      for (const [key, value] of Object.entries(initialState)) {
        state[key] = value
      }
    }

    return { state, clear, v$ }
  },
}
</script>
