<template>
<h3>NUESTRA TIENDA</h3>
<p class="textHome">Aquí se muestra el trabajo de los artesanos, cada una de ellas muestra
  que hacen y quienes son.
</p>
 <div class="column-start">
  <div class="card" style="width: 18rem;">
    <img src="@/assets/pulseras.jpg" class="card-img-top" alt="manillas">
    <div class="card-body">
     <h5 class="card-title">Artesano Luis</h5>
     <p class="card-text">Luis hace pulseras que son accesorios que exaltan la belleza de las personas que las usan...</p>
     <a href="#" class="btn btn-primary">Más información</a>
    </div>
  </div>
 </div>
 <div class="column-center">
  <div class="card" style="width: 18rem;">
    <img src="@/assets/mochilas.jpg" class="card-img-top" alt="manillas">
    <div class="card-body">
     <h5 class="card-title">Artesana Luisa</h5>
     <p class="card-text">Las mochilas más coloridas y de todos los tamaños puedes encontrarlas en el stund up de Luisa</p>
     <a href="#" class="btn btn-primary">Más información</a>
    </div>
  </div>
 </div>
 <div class="column-end">
  <div class="card" style="width: 18rem;">
    <img src="@/assets/okama.jpg" class="card-img-top" alt="manillas">
    <div class="card-body">
     <h5 class="card-title">Artesana Lucero</h5>
     <p class="card-text">La artesana Lucero construye las más bellas okamas, representativas de los indigenas del pais.</p>
     <a href="#" class="btn btn-primary">Más información</a>
    </div>
  </div>
 </div>
</template>

<script>
export default {
  name: 'ComponentHome'
}
</script>

<style>
  .column-start{
    float: left;
    width: 400px;
  }
  .column-center{
    float:left;
    width: 300px;
  }
   .column-end{
    float:right;
    width: 300px;
  }
  h3{
   text-align: center;
  }
  .textHome{
   text-align: center;
  }
</style>
