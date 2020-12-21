<template>
  <v-app>
    <v-app-bar
      app
      color="blue darken-4"
      dark
    >

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/mathiastop"
        target="_blank"
        text
      >
        <v-icon x-large>mdi-github</v-icon>
      </v-btn>
      <v-divider vertical inset></v-divider>
      <v-btn
        href="https://www.linkedin.com/in/mathias-top-93254a174/"
        target="_blank"
        text
      >
        <v-icon x-large>mdi-linkedin</v-icon>
      </v-btn>
      <v-divider vertical inset></v-divider>
      <v-btn
        href="mailto:mathiastop@epitech.eu"
        target="_blank"
        text
      >
        <v-icon x-large>mdi-email-edit</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <v-alert type="warning">
        Ce site est en construction.
      </v-alert>
    </v-main>

    <v-main>
      <Main/>
    </v-main>
    <v-divider></v-divider>
    <v-main>
      <Experience/>
    </v-main>
    <v-divider></v-divider>
    <v-main>
      <Formation/>
    </v-main>
    <v-divider></v-divider>
    <v-main>
      <Competences/>
    </v-main>
    <v-divider></v-divider>
    <v-main>
      <Contact/>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
import Main from './components/Main.vue'
import Experience from './components/Experience.vue'
import Formation from './components/Formation.vue'
import Competences from './components/Competences.vue'
import Contact from './components/Contact.vue'

export default Vue.extend({
  name: 'App',

  components: {
    Main,
    Experience,
    Formation,
    Competences,
    Contact
  },

  data: () => ({
    //
  })
})
</script>
