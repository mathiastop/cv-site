<template>
  <v-container>
    <v-row v-show="$vuetify.breakpoint.mdAndUp">
      <v-col cols="1"></v-col>
      <v-col cols="10">
        <div style="font-size: 130px; font-weight: bold; color: darkblue">
          FORMATION
        </div>
        <v-list>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Baccalauréat STI2D
              </v-list-item-title>
              <v-list-item-subtitle style="font-size: 30px">
                Lycée St Rémi - Roubaix - 2018
              </v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Expert en Technologie de l'Information
              </v-list-item-title>
              <v-list-item-subtitle>
                Epitech - Lille - 2023
              </v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-col>
    </v-row>

    <v-row v-show="$vuetify.breakpoint.smAndDown">
    <v-col cols="1"></v-col>
    <v-col cols="10">
      <div style="font-size: 130px; font-weight: bold; color: darkblue">
        FORMATION
      </div>
      <v-list>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title style="font-size: 70px; color: darkorange">
              Baccalauréat STI2D
            </v-list-item-title>
            <v-list-item-subtitle style="font-size: 30px">
              Lycée St Rémi - Roubaix - 2018
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title style="font-size: 70px; color: darkorange">
              Expert en Technologie de l'Information
            </v-list-item-title>
            <v-list-item-subtitle>
              Epitech - Lille - 2023
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-col>
  </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'Formation'
}
</script>

<style scoped>

</style>
