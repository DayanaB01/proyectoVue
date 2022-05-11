<template>
<div class="container">
  <p>*Si ya estas registrado sólo inicia sesión, si es primera vez
    que entras a nuestra plataforma, y deseas iniciar sesión primero
    debes llenar el formulario de registro.
  </p>
  <ComponentRegister/>
</div>
</template>

<script>
import ComponentRegister from '@/components/ComponentRegister.vue'

export default {
  name: 'LoginView',
  components: {
    ComponentRegister
  }
}
</script>
