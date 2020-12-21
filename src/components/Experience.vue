<template>
  <v-container>
    <p class="text-h1 blue--text text--darken-3 font-weight-bold">EXPERIENCES</p>
    <v-list-group>
      <template v-slot:activator>
        <v-list-item-title class="text-h2 orange--text text--darken-1 font-weight-bold">Développeur Web</v-list-item-title>
      </template>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h3 blue-grey--text text--darken-1">
            Mo&Jo - Lille - Juillet 2019/Octobre 2019
          </v-list-item-title>
          <v-list-item-subtitle class="text-h4 black--text">
            Migration de l’ensemble des projets sous la technologie <strong class="blue--text text--darken-3">Docker</strong>
          </v-list-item-subtitle>
          <v-list-item-subtitle class="text-h4 black--text">
            Réalisation de sites web en <strong class="blue--text text--darken-3">PHP</strong> avec le framework <strong class="blue--text text--darken-3">Symfony</strong>
          </v-list-item-subtitle>
          <v-list-item-subtitle class="text-h4 black--text">
            Réalisation d'une veille concernant l’intégration continue - <strong class="blue--text text--darken-3">PHPUnit</strong> et <strong class="blue--text text--darken-3">CircleCI</strong>
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </v-list-group>
    <v-list-group>
    <template v-slot:activator>
      <v-list-item-title class="text-h2 orange--text text--darken-1 font-weight-bold">Chef de projet</v-list-item-title>
    </template>
    <v-list-item>
      <v-list-item-content>
        <v-list-item-title class="text-h3 blue-grey--text text--darken-1">
          LUC Judo - Lille - Juin 2020/Août 2020
        </v-list-item-title>
        <v-list-item-subtitle class="text-h4 black--text">
          Réalisation d'un site en <strong class="blue--text text--darken-3">PHP/Symfony</strong> pour le back, et <strong class="blue--text text--darken-3">Boostrap</strong> pour le front
        </v-list-item-subtitle>
        <v-list-item-subtitle class="text-h4 black--text">
          <v-tooltip bottom>
            <template v-slot:activator="{on, attrs}">
              <span v-bind="attrs" v-on="on">
                <a href="https://lillejudo.fr" target="_blank" class="orange--text text--darken-1">
                  https://lillejudo.fr
                </a>
              </span>
            </template>
            <span>Ouvrir dans un nouvel onglet</span>
          </v-tooltip>
        </v-list-item-subtitle>
      </v-list-item-content>
    </v-list-item>
  </v-list-group>
  </v-container>
</template>

<script>
export default {
  name: 'Experience'
}
</script>

<style scoped>
.change-color:hover {
  color: darkorange;
}
</style>
