<template>
  <div class="container">
    <h1>¿Qué es Start.com?</h1>
    <ComponentDescription tittleDescription="Se crea..."/>
  </div>
</template>

<script>
import ComponentDescription from '@/components/ComponentDescription.vue'
export default {
  name: 'DescriptionView',
  components: {
    ComponentDescription
  }
}
</script>

<style>
 .container{
   height: 550px;
 }
</style>
