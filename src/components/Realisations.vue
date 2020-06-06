<template>
  <v-container>
    <v-row v-show="$vuetify.breakpoint.smAndUp">
      <v-col cols="1"></v-col>
      <v-col cols="10">
        <div style="font-size: 130px; font-weight: bold; color: darkblue">
          Réalisations
        </div>
        <v-list>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Sécurisation d'un lit à barreaux
              </v-list-item-title>
              <v-list-item-icon>
                <v-icon class="change-color" size="50">mdi-language-python</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                Projet réalisé afin de valider mon Baccalauréat.<br/>
                Création d'un API en Python, et mise en lien avec une Raspberry permettant de contrôler le lit.
              </v-list-item-content>
            </v-list-item-content>
          </v-list-item>
          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Organisation du Remot'Hackthon
              </v-list-item-title>
              <v-list-item-icon>
                <v-icon class="change-color" size="50">mdi-remote-desktop</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                Organisation d'un hackathon sur le thème du travail en remote à destination des étudiants d'Epitech Lille.<br/>
                Comment, par rapport au confinement et aux problématiques majeures en entreprise, pouvons-nous pallier la distance et le manque d’interactions entre les personnes au sein des groupes de collaborateurs ?
              </v-list-item-content>
            </v-list-item-content>
          </v-list-item>
          <v-list-item three-line>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Création de différents sites Web
              </v-list-item-title>
              <v-list-item-icon>
                <v-icon class="change-color" size="50">mdi-language-php</v-icon>
                <v-icon class="change-color" size="50">mdi-symfony</v-icon>
                <v-divider vertical/>
                <v-icon class="change-color" size="50">mdi-vuejs</v-icon>
                <v-icon class="change-color" size="50">mdi-vuetify</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                Réalisation d'un site e-commerce de code de promotion en PHP avec le framework Symfony - promodisiac.com<br/>
                Réalisation de mon site personnel en VueJS avec le framework Vuetify - mathiastop.eu
              </v-list-item-content>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-col>
    </v-row>
    <v-row v-show="$vuetify.breakpoint.smAndUp">
      <v-col cols="1"></v-col>
      <v-col cols="10">
        <div style="font-size: 130px; font-weight: bold; color: darkblue">
          Réalisations
        </div>
        <v-list>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Sécurisation d'un lit à barreaux
              </v-list-item-title>
              <v-list-item-icon>
                <v-icon class="change-color" size="50">mdi-language-python</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                Projet réalisé afin de valider mon Baccalauréat.<br/>
                Création d'un API en Python, et mise en lien avec une Raspberry permettant de contrôler le lit.
              </v-list-item-content>
            </v-list-item-content>
          </v-list-item>
          <v-list-item two-line>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Organisation du Remot'Hackthon
              </v-list-item-title>
              <v-list-item-icon>
                <v-icon class="change-color" size="50">mdi-remote-desktop</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                Organisation d'un hackathon sur le thème du travail en remote à destination des étudiants d'Epitech Lille.<br/>
                Comment, par rapport au confinement et aux problématiques majeures en entreprise, pouvons-nous pallier la distance et le manque d’interactions entre les personnes au sein des groupes de collaborateurs ?
              </v-list-item-content>
            </v-list-item-content>
          </v-list-item>
          <v-list-item three-line>
            <v-list-item-content>
              <v-list-item-title style="font-size: 70px; color: darkorange">
                Création de différents sites Web
              </v-list-item-title>
              <v-list-item-icon>
                <v-icon class="change-color" size="50">mdi-language-php</v-icon>
                <v-icon class="change-color" size="50">mdi-symfony</v-icon>
                <v-divider vertical/>
                <v-icon class="change-color" size="50">mdi-vuejs</v-icon>
                <v-icon class="change-color" size="50">mdi-vuetify</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                Réalisation d'un site e-commerce de code de promotion en PHP avec le framework Symfony - promodisiac.com<br/>
                Réalisation de mon site personnel en VueJS avec le framework Vuetify - mathiastop.eu
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
  name: 'Realisations'
}
</script>

<style scoped>
.change-color:hover {
  color: darkblue;
}
</style>
