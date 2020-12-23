<template>
  <v-app>
    <v-app-bar
      app
      color="blue darken-4"
      dark
    >
      <div>
        <v-btn text x-large @click="$vuetify.goTo('#index')">
          Index
        </v-btn>
        <v-btn text x-large @click="$vuetify.goTo('#experiences')">
          Experiences
        </v-btn>
        <v-btn text x-large @click="$vuetify.goTo('#formations')">
          Formations
        </v-btn>
        <v-btn text x-large @click="$vuetify.goTo('#competences')">
          Compétences
        </v-btn>
        <v-btn text x-large @click="$vuetify.goTo('#contact')">
          Contact
        </v-btn>
      </div>
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

    <v-main id="index">
      <Main/>
    </v-main>
    <v-divider></v-divider>
    <v-main id="experiences">
      <Experience/>
    </v-main>
    <v-divider></v-divider>
    <v-main id="formations">
      <Formation/>
    </v-main>
    <v-divider></v-divider>
    <v-main id="competences">
      <Competences/>
    </v-main>
    <v-divider></v-divider>
    <v-main id="contact">
      <Contact/>
    </v-main>
    <v-footer color="blue darken-4" dark padless>
      <v-row
        justify="center"
      >
        <div>
          <v-btn text x-large @click="$vuetify.goTo('#index')">
            Index
          </v-btn>
          <v-btn text x-large @click="$vuetify.goTo('#experiences')">
            Experiences
          </v-btn>
          <v-btn text x-large @click="$vuetify.goTo('#formations')">
            Formations
          </v-btn>
          <v-btn text x-large @click="$vuetify.goTo('#competences')">
            Compétences
          </v-btn>
          <v-btn text x-large @click="$vuetify.goTo('#contact')">
            Contact
          </v-btn>
        </div>
        <v-col
          class="text-center"
          cols="12"
        >
          {{ new Date().getFullYear() }} — <strong>© Mathias Top</strong>
        </v-col>
      </v-row>
    </v-footer>
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
