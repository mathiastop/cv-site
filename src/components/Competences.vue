<template>
    <v-container>
      <v-row v-show="$vuetify.breakpoint.mdAndUp">
        <v-col cols="1"></v-col>
        <v-col cols="10">
          <div style="font-size: 130px; font-weight: bold; color: darkblue">
            Compétences
          </div>
          <v-list>
            <v-list-item>
              <v-icon size="100" class="change-color">mdi-docker</v-icon>
              <v-icon size="100" class="change-color">mdi-kubernetes</v-icon>
              <v-divider vertical/>
              <v-icon size="100" class="change-color">mdi-language-php</v-icon>
              <v-icon size="100" class="change-color">mdi-symfony</v-icon>
              <v-divider vertical/>
              <v-icon size="100" class="change-color">mdi-vuejs</v-icon>
              <v-icon size="100" class="change-color">mdi-vuetify</v-icon>
              <v-divider vertical/>
              <v-icon size="100" class="change-color">mdi-language-c</v-icon>
              <v-icon size="100" class="change-color">mdi-language-cpp</v-icon>
              <v-icon size="100" class="change-color">mdi-language-python</v-icon>
            </v-list-item>
          </v-list>
        </v-col>
      </v-row>
    </v-container>
</template>

<script>
export default {
  name: 'Competences'
}
</script>

<style scoped>
.change-color:hover {
  color: darkorange;
}
</style>
