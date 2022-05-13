<template>
<div class="container">
  <p>*Si ya estas registrado sólo inicia sesión, si es primera vez
    que entras a nuestra plataforma, y deseas iniciar sesión primero
    debes llenar el formulario de registro.
  </p>
  <ComponentRegister :name="profile.name" :lastname="profile.lastname"
     :email="profile.email" :password="profile.password" @getData="getData"/>
</div>
</template>

<script>
import ComponentRegister from '@/components/ComponentRegister.vue'

export default {
  name: 'LoginView',
  components: {
    ComponentRegister
  },
  data () {
    return {
      profile: {
        name: 'Dayana',
        lastname: 'Betancur',
        email: 'dayana@gmail.com',
        password: '12345'
      }
    }
  },
  methods: {
    getData (informacion) {
      this.profile.name = informacion.name
      this.profile.lastname = informacion.lastname
      this.profile.email = informacion.email
      this.profile.password = informacion.password
    }
  }
}
</script>
