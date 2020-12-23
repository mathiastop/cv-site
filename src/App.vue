<template>
  <v-app>
    <v-app-bar
      class="d-md-block d-none"
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
        <v-icon large>mdi-github</v-icon>
      </v-btn>
      <v-divider vertical inset></v-divider>
      <v-btn
        href="https://www.linkedin.com/in/mathias-top-93254a174/"
        target="_blank"
        text
      >
        <v-icon large>mdi-linkedin</v-icon>
      </v-btn>
      <v-divider vertical inset></v-divider>
      <v-btn
        href="mailto:mathiastop@epitech.eu"
        target="_blank"
        text
      >
        <v-icon large>mdi-email-edit</v-icon>
      </v-btn>
      <v-divider vertical inset></v-divider>
      <v-btn
        href="tel:06.05.26.20.77"
        target="_blank"
        text
      >
        <v-icon large>mdi-phone-ring</v-icon>
      </v-btn>
    </v-app-bar>
    <v-app-bar
      class="d-md-none d-block"
      app
      color="blue darken-4"
      dark
    >
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      <v-spacer></v-spacer>
      <v-btn
        href="https://github.com/mathiastop"
        target="_blank"
        text
      >
        <v-icon large>mdi-github</v-icon>
      </v-btn>
      <v-divider vertical inset></v-divider>
      <v-btn
        href="https://www.linkedin.com/in/mathias-top-93254a174/"
        target="_blank"
        text
      >
        <v-icon large>mdi-linkedin</v-icon>
      </v-btn>
      <v-divider vertical inset></v-divider>
      <v-btn
        href="mailto:mathiastop@epitech.eu"
        target="_blank"
        text
      >
        <v-icon large>mdi-email-edit</v-icon>
      </v-btn>
      <v-divider vertical inset></v-divider>
      <v-btn
        href="tel:06.05.26.20.77"
        target="_blank"
        text
      >
        <v-icon large>mdi-phone-ring</v-icon>
      </v-btn>
    </v-app-bar>
    <v-navigation-drawer
      v-model="drawer"
      :class="$vuetify.breakpoint.mdAndUp ? 'd-none' : 'd-block'"
      color="blue darken-4"
      dark
      app
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
        >
          <v-list-item>
            <v-list-item-title @click="$vuetify.goTo('#index'), drawer = !drawer">Index</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title @click="$vuetify.goTo('#experiences'), drawer = !drawer">Experiences</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title @click="$vuetify.goTo('#formations'), drawer = !drawer">Formations</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title @click="$vuetify.goTo('#competences'), drawer = !drawer">Compétences</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title @click="$vuetify.goTo('#contact'), drawer = !drawer">Contact</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
    <br/>
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
        <div class="d-sm-block d-none">
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
    drawer: false,
    group: null
  })
})
</script>
