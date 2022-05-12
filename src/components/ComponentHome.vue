<template>
<h3>NUESTRA TIENDA</h3>
<p class="textHome">Aquí se muestra el trabajo de los artesanos,
  cada una de ellas muestra que hacen y quienes son.
</p>
 <div class="column-start">
  <div class="card" style="width: 18rem;">
    <img src="@/assets/pulseras.jpg" class="card-img-top" alt="manillas">
    <div class="card-body">
     <h5 class="card-title">Artesano Luis</h5>
     <p class="card-text">Luis hace pulseras que son accesorios que exaltan
       la belleza de las personas que las usan...</p>
     <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#staticBackdrop">
      Más información
     </button>
      <div class="modal fade" id="staticBackdrop" data-bs-backdrop="static"
       data-bs-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
       <div class="modal-dialog">
        <div class="modal-content">
         <div class="modal-header">
          <h5 class="modal-title" id="staticBackdropLabel">Luis- Alfarero</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
         </div>
         <div class="modal-body">
          <p>Originario de comunidad etnica asentueda en el occidente de Caldas, tiene 55 años de
            los cuales 45 han sido dedicados a la agricultura y la artesania, habilidades que cual heredo de sus
            ancestros. Luis en parte de su tiempo se de didica a ser alfarero, arte que lo ha ayudado
            a adquirir ingresos economicos para el bien estar de su familia.
            Comunicate con Luis y adquiere de los más hermosos productos de la alfareria colombiana.
            3134543245-344335678.
          </p>
         </div>
        </div>
       </div>
      </div>
    </div>
  </div>
 </div>
 <div class="column-center">
  <div class="card" style="width: 18rem;">
    <img src="@/assets/mochilas.jpg" class="card-img-top" alt="manillas">
    <div class="card-body">
     <h5 class="card-title">Artesana Luisa</h5>
     <p class="card-text">Las mochilas más coloridas y de todos los tamaños puedes encontrarlas en
       el stund up de Luisa</p>
     <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#staticBackdrops">
      Más información
     </button>
      <div class="modal fade" id="staticBackdrops" data-bs-backdrop="static" data-bs-keyboard="false"
       tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
       <div class="modal-dialog">
        <div class="modal-content">
         <div class="modal-header">
          <h5 class="modal-title" id="staticBackdropLabel">Luisa- Tejedora</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
         </div>
         <div class="modal-body">
          <p>Luisa es una joven tejedora que a pesar de su corta edad se a dedicado a tejer
            mochilas, las cuales vende en el mercado de su pueblo natal. De esta manera Luisa
            a contribuido en la economia de su hogar, adémas enseña el arte de tejer a los niños
            que viven en su pueblo.<br>
            Si deseas comprar una de estas hermosas mochilas, comunicate con Luisa y adquierelas
            directamente: 321453356-54322346.
          </p>
         </div>
        </div>
       </div>
      </div>
    </div>
  </div>
 </div>
 <div class="column-end">
  <div class="card" style="width: 18rem;">
    <img src="@/assets/okama.jpg" class="card-img-top" alt="manillas">
    <div class="card-body">
     <h5 class="card-title">Artesana Lucero</h5>
     <p class="card-text">La artesana Lucero construye las más bellas okamas, representativas
       de los indigenas del pais.</p>
     <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#staticBackdropx">
      Más información
     </button>
      <div class="modal fade" id="staticBackdropx" data-bs-backdrop="static" data-bs-keyboard="false"
      tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
       <div class="modal-dialog">
        <div class="modal-content">
         <div class="modal-header">
          <h5 class="modal-title" id="staticBackdropLabel">Lucero -Artesana</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
         </div>
         <div class="modal-body">
          La artesana Lucero es una madre cabeza de familia, que gracias al arte que aprendio de su familia,
          ha podido vivir economicamente dando estudio a sus hijos, todos los accesorios que hace los vende
          en los eventos de artesania que se hacen cerca del pueblo donde reside y del cual es también
          oriunda.<br>
          Si deseas adquirir uno de sus productos y contribuir con la economia de Lucer, comunicate
          con ella: 321546466-3146785443.
         </div>
        </div>
       </div>
      </div>
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
   color: black;
   font-family: cursive;
  }
  h5{
    color: black;
    font-family: cursive;
  }
  .textHome{
   text-align: center;
  }
  p{
    color:black;
    font-size: 1rem;
  }
</style>
