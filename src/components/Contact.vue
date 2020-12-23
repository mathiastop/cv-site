<template>
  <v-container>
    <p class="
      text-md-h1
      text-sm-h2
      text-h4
      blue--text text--darken-4 font-weight-bold">
      CONTACT
    </p>
    <v-alert type="success" :value="sendMail" dismissible transition="slide-y-transition" @click="sendMail = false">
      Votre message a été envoyé.
    </v-alert>
    <v-alert type="error" :value="errorMail" dismissible transition="slide-y-transition" @click="errorMail = false">
      Une erreur est survenue lors de l'envoi de votre message.
    </v-alert>
    <v-row>
      <v-col md="6">
        <v-form
          ref="form"
          v-model="valid"
          lazy-validation
          @submit.prevent="sendEmail"
        >
          <v-text-field
            ref="name"
            name="formName"
            v-model="name"
            :counter="50"
            :rules="nameRules"
            label="Nom/Prénom *"
            required
          ></v-text-field>
          <v-text-field
            ref="email"
            name="formEmail"
            v-model="email"
            :rules="emailRules"
            label="E-mail *"
            required
          ></v-text-field>
          <v-text-field
            ref="subject"
            name="formSubject"
            v-model="subject"
            :rules="subjectRules"
            label="Sujet *"
            required
          ></v-text-field>
          <v-textarea
            ref="message"
            name="formMessage"
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
            type="submit"
            value="Send"
          >
            Valider
          </v-btn>
          <v-btn
            color="error"
            class="mr-4"
            @click="reset"
          >
            Effacer formulaire
          </v-btn>
        </v-form>
      </v-col>
      <v-col md="6">
        <v-row justify="center">
          <v-col md="6">
            <v-tooltip top>
              <template v-slot:activator="{on, attrs}">
                <span v-bind="attrs" v-on="on">
                  <v-layout justify-center>
                    <v-hover v-slot="{hover}">
                      <a href="https://github.com/mathiastop" target="_blank" class="text-decoration-none">
                        <v-icon :size="$vuetify.breakpoint.smAndDown ? 160 : 200" :color="hover ? 'black' : ''">mdi-github</v-icon>
                      </a>
                    </v-hover>
                  </v-layout>
                </span>
              </template>
              <span>Ouvrir dans un nouvel onglet</span>
            </v-tooltip>
          </v-col>
          <v-col md="6">
            <v-tooltip top>
              <template v-slot:activator="{on, attrs}">
                <span v-bind="attrs" v-on="on">
                  <v-layout justify-center>
                    <v-hover v-slot="{hover}">
                      <a href="https://www.linkedin.com/in/mathias-top-93254a174/" target="_blank" class="text-decoration-none">
                        <v-icon :size="$vuetify.breakpoint.smAndDown ? 160 : 200" :color="hover ? 'blue darken-3' : ''">mdi-linkedin</v-icon>
                      </a>
                    </v-hover>
                  </v-layout>
                </span>
              </template>
              <span>Ouvrir dans un nouvel onglet</span>
            </v-tooltip>
          </v-col>
          <v-col md="6">
            <v-tooltip top>
              <template v-slot:activator="{on, attrs}">
                <span v-bind="attrs" v-on="on">
                  <v-layout justify-center>
                    <v-hover v-slot="{hover}">
                      <a href="mailto:mathiastop@epitech.eu" class="text-decoration-none">
                        <v-icon :size="$vuetify.breakpoint.smAndDown ? 160 : 200" :color="hover ? 'orange' : ''">mdi-email-edit</v-icon>
                      </a>
                    </v-hover>
                  </v-layout>
                </span>
              </template>
              <span>mathias.top@epitech.eu</span>
            </v-tooltip>
          </v-col>
          <v-col md="6">
            <v-tooltip top>
              <template v-slot:activator="{on, attrs}">
                <span v-bind="attrs" v-on="on">
                  <v-layout justify-center>
                    <v-hover v-slot="{hover}">
                      <a href="tel:06.05.26.20.77" class="text-decoration-none">
                        <v-icon :size="$vuetify.breakpoint.smAndDown ? 160 : 200" :color="hover ? 'blue-grey darken-1' : ''">mdi-phone-ring</v-icon>
                      </a>
                    </v-hover>
                  </v-layout>
                </span>
              </template>
              <span>06.05.26.20.77</span>
            </v-tooltip>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import emailjs from 'emailjs-com'
export default {
  name: 'Contact',

  data: () => ({
    sendMail: false,
    errorMail: false,
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
    },
    sendEmail (e) {
      const name = this.$refs.name.value
      const email = this.$refs.email.value
      const subject = this.$refs.subject.value
      const message = this.$refs.message.value
      try {
        emailjs.sendForm('service_ch0km4a', 'template_7yhev7r', e.target,
          'user_EkUqCpfhOPkjZ3jWJez0h', {
            formName: name,
            formEmail: email,
            formSubject: subject,
            formMessage: message
          })
        this.$refs.form.reset()
        this.sendMail = true
        window.setTimeout(() => {
          this.sendMail = false
        }, 5000)
      } catch (error) {
        console.log('ERROR: ' + error)
        this.errorMail = true
        window.setTimeout(() => {
          this.errorMail = false
        }, 5000)
      }
    },
    reset () {
      this.$refs.form.reset()
    }
  }
}
</script>

<style scoped>

</style>
