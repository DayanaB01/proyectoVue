<template>
<div>
  <nav class="navbar navbar-light">
    <div class="container-fluid">
      <h1>Start.com</h1>
      <ul class="nav justify-content-end">
        <li class="nav-item">
          <router-link to="/">Inicio</router-link> |
        </li>
        <li class="nav-item">
          <router-link to="/description">Nosotros</router-link> |
        </li>
        <li class="nav-item">
          <router-link to="/login">Iniciar Sesion</router-link>
        </li>
      </ul>
    </div>
  </nav>
  <router-view />
  </div>
  <footerComponent/>
</template>

<script>
import footerComponent from '@/components/layers/footerComponent.vue'

export default {
  name: 'App',
  components: {
    footerComponent
  }
}
</script>

<style>
.navbar {
  background-color: burlywood;
}
h1{
  color: black;
  font-family: cursive;
}
</style>
