<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
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
      <v-btn
        href="https://www.linkedin.com/in/mathias-top-93254a174/"
        target="_blank"
        text
      >
        <v-icon x-large>mdi-linkedin</v-icon>
      </v-btn>
    </v-app-bar>

    <!--<v-content>
      <HelloWorld/>
    </v-content>-->
    <v-content>
      <Main/>
    </v-content>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
import Main from './components/Main.vue'

export default Vue.extend({
  name: 'App',

  components: {
    Main
  },

  data: () => ({
    //
  })
})
</script>
