<template>
  <v-container>
    <v-row v-show="$vuetify.breakpoint.mdAndUp">
      <v-col cols="1"></v-col>
      <v-col cols="10">
        <div style="font-size: 130px; font-weight: bold; color: darkblue">
          EXPERIENCE
        </div>
        <v-list>

          <v-list-item>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Développeur Web
              </v-list-item-title>
              <v-list-item-subtitle style="font-size: 30px">
                Mo&Jo - Lille - Juillet 2019/Octobre 2019
              </v-list-item-subtitle>
              <v-list-item-content>
                Migrations de l'ensemble des projets sous la technologie Docker<br/>
                Réalisation de site web en PHP avec le framework Symfony<br/>
                Réalisation d'un veille concernant l'intégration continue<br/>
              </v-list-item-content>
            </v-list-item-content>
          </v-list-item>

          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Rayonnage
              </v-list-item-title>
              <v-list-item-subtitle style="font-size: 30px">
                Auchan - Villeneuve d'Ascq - Juillet 2017/Août 2017
              </v-list-item-subtitle>
              <v-list-item-content>
                Mise en rayon d'article de jeux vidéos
              </v-list-item-content>
            </v-list-item-content>
          </v-list-item>

        </v-list>
      </v-col>
    </v-row>
    <v-row v-show="$vuetify.breakpoint.smAndDown">
      <v-col cols="1"></v-col>
      <v-col cols="10">
        <div style="font-size: 130px; font-weight: bold; color: darkblue">
          EXPERIENCE
        </div>
        <v-list>

          <v-list-item>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Rayonnage
              </v-list-item-title>
              <v-list-item-subtitle style="font-size: 30px">
                Auchan - Villeneuve d'Ascq - Juillet 2017/Août 2017
              </v-list-item-subtitle>
              <v-list-item-content>
                Mise en rayon d'article de jeux vidéos
              </v-list-item-content>
            </v-list-item-content>
          </v-list-item>

          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Développeur Web
              </v-list-item-title>
              <v-list-item-subtitle style="font-size: 30px">
                Mo&Jo - Lille - Juillet 2019/Octobre 2019
              </v-list-item-subtitle>
              <v-list-item-content>
                Migrations de l'ensemble des projets sous la technologie Docker<br/>
                Réalisation de site web en PHP avec le framework Symfony<br/>
                Réalisation d'un veille concernant l'intégration continue<br/>
              </v-list-item-content>
            </v-list-item-content>
          </v-list-item>

        </v-list>
      </v-col>
    </v-row>
  </v-container>

</template>

<script>
export default {
  name: 'Experience'
}
</script>

<style scoped>

</style>
