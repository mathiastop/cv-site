<template>
  <v-container>
    <p class="
      text-md-h1
      text-sm-h2
      text-h4
      blue--text text--darken-4 font-weight-bold">
      EXPERIENCES
    </p>
    <v-list-group>
      <template v-slot:activator>
        <v-list-item-title class="text-wrap
          text-md-h2
          text-sm-h3
          text-h4
          orange--text text--darken-1 font-weight-bold">
          Développeur Web
        </v-list-item-title>
      </template>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-wrap
            text-md-h3
            text-sm-h4
            text-h5
            blue-grey--text text--darken-1">
            Mo&Jo | Lille | Juillet 2019/Octobre 2019
          </v-list-item-title>
          <v-list-item-subtitle class="text-wrap
            text-md-h4
            text-sm-h5
            text-h6
            black--text">
            <ul>
              <li>
                Migration de l’ensemble des projets sous la technologie <strong class="blue--text text--darken-4">Docker</strong>
              </li>
            </ul>
          </v-list-item-subtitle>
          <v-list-item-subtitle class="text-wrap
            text-md-h4
            text-sm-h5
            text-h6
            black--text">
            <ul>
              <li>
                Réalisation de sites web en <strong class="blue--text text--darken-4">PHP</strong> avec le framework <strong class="blue--text text--darken-4">Symfony</strong>
              </li>
            </ul>
          </v-list-item-subtitle>
          <v-list-item-subtitle class="text-wrap
            text-md-h4
            text-sm-h5
            text-h6
            black--text">
            <ul>
              <li>
                Réalisation d'une veille concernant l’intégration continue - <strong class="blue--text text--darken-4">PHPUnit</strong> et <strong class="blue--text text--darken-4">CircleCI</strong>
              </li>
            </ul>
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </v-list-group>
    <v-list-group>
    <template v-slot:activator>
      <v-list-item-title class="text-wrap
        text-md-h2
        text-sm-h3
        text-h4
        orange--text text--darken-1 font-weight-bold">
        Chef de projet
      </v-list-item-title>
    </template>
    <v-list-item>
      <v-list-item-content>
        <v-list-item-title class="text-wrap
          text-md-h3
          text-sm-h4
          text-h5
          blue-grey--text text--darken-1">
          LUC Judo | Lille | Juin 2020/Août 2020
        </v-list-item-title>
        <v-list-item-subtitle class="text-wrap
            text-md-h4
            text-sm-h5
            text-h6
            black--text">
          <ul>
            <li>
              Réalisation d'un site en <strong class="blue--text text--darken-4">PHP/Symfony</strong> pour le back, et <strong class="blue--text text--darken-4">Boostrap</strong> pour le front
            </li>
          </ul>
        </v-list-item-subtitle>
        <v-list-item-subtitle class="
            text-md-h4
            text-sm-h5
            text-h6
            black--text">
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

</style>
