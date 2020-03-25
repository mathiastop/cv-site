<template>
  <v-app>
    <v-app-bar
      app
      color="#17358B"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Mathias Top"
          class="shrink mr-2"
          contain
          src="./assets/mathias.top.png"
          transition="scale-transition"
          width="40"
        />
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
    </v-app-bar>

    <v-content>
      <v-alert type="warning">
        Ce site est en construction.
      </v-alert>
    </v-content>

    <v-content>
      <Main/>
    </v-content>
    <v-divider></v-divider>
    <v-content>
      <Experience/>
    </v-content>
    <v-divider></v-divider>
    <v-content>
      <Formation/>
    </v-content>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
import Main from './components/Main.vue'
import Experience from './components/Experience.vue'
import Formation from './components/Formation.vue'

export default Vue.extend({
  name: 'App',

  components: {
    Main,
    Experience,
    Formation
  },

  data: () => ({
    //
  })
})
</script>
