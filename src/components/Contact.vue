<template>
  <v-container>
    <p class="text-h1 blue--text text--darken-4 font-weight-bold">CONTACT</p>
    <v-row>
      <v-col md="6">
        <v-form
          ref="form"
          v-model="valid"
          lazy-validation
        >
          <v-text-field
            ref="name"
            v-model="name"
            :counter="50"
            :rules="nameRules"
            label="Nom/Prénom *"
            required
          ></v-text-field>
          <v-text-field
            ref="email"
            v-model="email"
            :rules="emailRules"
            label="E-mail *"
            required
          ></v-text-field>
          <v-text-field
            ref="subject"
            v-model="subject"
            :rules="subjectRules"
            label="Sujet *"
            required
          ></v-text-field>
          <v-textarea
            ref="message"
            v-model="message"
            :counter="500"
            :rules="messageRules"
            label="Message *"
            required
          ></v-textarea>
          <v-btn
            :disabled="!valid"
            color="blue darken-3 white--text"
            class="mr-4"
            @click="validate"
          >
            Valider
          </v-btn>
          <v-btn
            color="error"
            class="mr-4"
            @click="reset"
          >
            Réinitialiser formulaire
          </v-btn>
          <v-btn
            color="warning"
            @click="resetValidation"
          >
            Réinitialiser validations
          </v-btn>
        </v-form>
      </v-col>
      <v-col md="6">
        <v-row justify="center">
          <v-col md="6">
            <v-tooltip bottom>
              <template v-slot:activator="{on, attrs}">
                <span v-bind="attrs" v-on="on">
                  <v-layout justify-center>
                    <v-hover v-slot="{hover}">
                      <a href="https://github.com/mathiastop" target="_blank" style="text-decoration:none;">
                        <v-icon size="200" :color="hover ? 'black' : ''">mdi-github</v-icon>
                      </a>
                    </v-hover>
                  </v-layout>
                </span>
              </template>
              <span>Ouvrir dans un nouvel onglet</span>
            </v-tooltip>
          </v-col>
          <v-col md="6">
            <v-tooltip bottom>
              <template v-slot:activator="{on, attrs}">
                <span v-bind="attrs" v-on="on">
                  <v-layout justify-center>
                    <v-hover v-slot="{hover}">
                      <a href="https://www.linkedin.com/in/mathias-top-93254a174/" target="_blank" style="text-decoration:none;">
                        <v-icon size="200" :color="hover ? 'blue darken-3' : ''">mdi-linkedin</v-icon>
                      </a>
                    </v-hover>
                  </v-layout>
                </span>
              </template>
              <span>Ouvrir dans un nouvel onglet</span>
            </v-tooltip>
          </v-col>
          <v-col md="6">
            <v-tooltip bottom>
              <template v-slot:activator="{on, attrs}">
                <span v-bind="attrs" v-on="on">
                  <v-layout justify-center>
                    <v-hover v-slot="{hover}">
                      <a href="mailto:mathiastop@epitech.eu" style="text-decoration:none;">
                        <v-icon size="200" :color="hover ? 'orange' : ''">mdi-email-edit</v-icon>
                      </a>
                    </v-hover>
                  </v-layout>
                </span>
              </template>
              <span>Me contacter par mail</span>
            </v-tooltip>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'Contact',

  data: () => ({
    valid: true,
    name: '',
    nameRules: [
      v => !!v || 'Votre nom/prénom est requis',
      v => (v && v.length <= 50) || 'Votre nom/prénom ne doit pas excéder 50 caractères'
    ],
    email: '',
    emailRules: [
      v => !!v || 'Votre e-mail est requis',
      v => /.+@.+\..+/.test(v) || 'Votre e-mail doit être valide'
    ],
    subject: '',
    subjectRules: [
      v => !!v || 'Un sujet est requis'
    ],
    message: '',
    messageRules: [
      v => !!v || 'Un message est requis',
      v => (v && v.length <= 500) || 'Votre message ne peut pas excéder 500 caractères'
    ]
  }),

  methods: {
    validate () {
      this.$refs.form.validate()
      // const name = this.$refs.name.value
      // const email = this.$refs.email.value
      // const subject = this.$refs.subject.value
      // const message = this.$refs.message.value
    },
    reset () {
      this.$refs.form.reset()
    },
    resetValidation () {
      this.$refs.form.resetValidation()
    }
  }
}
</script>

<style scoped>

</style>
