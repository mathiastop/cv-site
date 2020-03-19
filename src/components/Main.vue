<template>
  <v-container>
    <v-row v-show="$vuetify.breakpoint.mdAndUp">
      <v-col cols="1" ></v-col>
      <v-col cols="10">
        <div style="font-size: 130px; font-weight: bold; color: darkblue">
          MATHIAS TOP
        </div>
        <div style="font-size: 70px; color: darkorange">
          Etudiant en Informatique
        </div>
        <div style="font-size: 25px">
          06.05.26.20.77 - mathias.top@epitech.eu
        </div>
        <br/>
        <div style="font-size: 20px; color: darkgrey">
          Etudiant en deuxième année à EPITECH Lille, je suis à la recherche d'un contrat de professionnalisation pour janvier 2021.
        </div>
      </v-col>
      <v-col cols="1"></v-col>
    </v-row>

    <v-row v-show="$vuetify.breakpoint.smAndDown">
      <v-col cols="1" ></v-col>
      <v-col cols="10">
        <div style="font-size: 130px; font-weight: bold; color: darkblue">
          MATHIAS TOP
        </div>
        <div style="font-size: 70px; color: darkorange">
          Etudiant en Informatique
        </div>
        <div style="font-size: 25px">
          06.05.26.20.77 - mathias.top@epitech.eu
        </div>
        <div style="font-size: 20px; color: darkgrey">
          Etudiant en deuxième année à EPITECH Lille, je suis à la recherche d'un contrat de professionnalisation pour janvier 2021.
        </div>
      </v-col>
      <v-col cols="1"></v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'Main'
}
</script>

<style scoped>

</style>
