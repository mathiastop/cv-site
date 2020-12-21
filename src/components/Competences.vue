<template>
    <v-container>
      <p class="text-h1 blue--text text--darken-4 font-weight-bold">COMPETENCES</p>
      <v-row>
        <v-col md="4">
          <v-list-group>
            <template v-slot:activator>
              <v-hover v-slot="{hover}">
                <v-list-item-title>
                  <v-layout justify-center>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-language-php</v-icon>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-symfony</v-icon>
                  </v-layout>
                </v-list-item-title>
              </v-hover>
            </template>
            <v-list-item-content>
              <p class="text-h4 black--text">
                Réalisation de plusieurs sites web
              </p>
            </v-list-item-content>
          </v-list-group>
        </v-col>
        <v-col md="4">
          <v-list-group>
            <template v-slot:activator>
              <v-hover v-slot="{hover}">
                <v-list-item-title>
                  <v-layout justify-center>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-docker</v-icon>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-kubernetes</v-icon>
                  </v-layout>
                </v-list-item-title>
              </v-hover>
            </template>
            <v-list-item-content>
              <p class="text-h4 black--text">
                Préparation de fichier de configuration pour le déploiment de différentes applications web
              </p>
            </v-list-item-content>
          </v-list-group>
        </v-col>
        <v-col md="4">
          <v-list-group>
            <template v-slot:activator>
              <v-hover v-slot="{hover}">
                <v-list-item-title>
                  <v-layout justify-center>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-bootstrap</v-icon>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-language-javascript</v-icon>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-jquery</v-icon>
                  </v-layout>
                </v-list-item-title>
              </v-hover>
            </template>
            <v-list-item-content>
              <p class="text-h4 black--text">
                Réalisation d'un JobBoard
              </p>
            </v-list-item-content>
          </v-list-group>
        </v-col>
        <v-col md="4">
          <v-list-group>
            <template v-slot:activator>
              <v-hover v-slot="{hover}">
                <v-list-item-title>
                  <v-layout justify-center>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-ansible</v-icon>
                  </v-layout>
                </v-list-item-title>
              </v-hover>
            </template>
            <v-list-item-content>
              <p class="text-h4 black--text">
                Automatisation de tâches complexes
              </p>
            </v-list-item-content>
          </v-list-group>
        </v-col>
        <v-col md="4">
          <v-list-group>
            <template v-slot:activator>
              <v-hover v-slot="{hover}">
                <v-list-item-title>
                  <v-layout justify-center>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-language-c</v-icon>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-language-cpp</v-icon>
                  </v-layout>
                </v-list-item-title>
              </v-hover>
            </template>
            <v-list-item-content>
              <p class="text-h4 black--text">
                Réalisations de plusieurs projets au sein d'Epitech
              </p>
            </v-list-item-content>
          </v-list-group>
        </v-col>
        <v-col md="4">
          <v-list-group>
            <template v-slot:activator>
              <v-hover v-slot="{hover}">
                <v-list-item-title>
                  <v-layout justify-center>
                    <v-icon size="100" :color="hover ? 'orange' : ''">mdi-language-java</v-icon>
                  </v-layout>
                </v-list-item-title>
              </v-hover>
            </template>
            <v-list-item-content>
              <p class="text-h4 black--text">
                Réalisation d'un Dashboard
              </p>
            </v-list-item-content>
          </v-list-group>
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

</style>
