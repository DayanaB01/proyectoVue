<template>
  <div class="container">
    <h2>¿Qué es Start.com?</h2>
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
 h2{
   font-size: 5px;
 }
</style>
