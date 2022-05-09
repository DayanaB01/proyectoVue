<template>
  <div class="column-right">
    <div id="carouselExampleSlidesOnly" class="carousel slide" data-bs-ride="carousel">
      <div class="carousel-inner">
        <div class="carousel-item active">
         <img src="@/assets/manillas.jpg" class="d-block w-90" alt="manillas">
        </div>
        <div class="carousel-item">
         <img src="@/assets/Medellín.jpg" class="d-block w-90" alt="mochilas">
        </div>
        <div class="carousel-item">
         <img src="@/assets/Sombrero.jpg" class="d-block w-90" alt="sombrero">
        </div>
     </div>
   </div>
  </div>
  <div class="column-left">
    <h1> {{ tittleDescription }} </h1>
    <p>
    ...una plataforma digital con el objetivo de <br>
    ayudarte a vender los productos artesanales que<br>
    haces con arduo trabajo, con creatividad y amor.<br>
    Asi muchas personas de todo el mundo puedan ver <br>
    y comprar tu producto.<br>
    <br>
    ¿Porque?...<br>
    Haciendo uso de la tecnologia se comercializan <br>
    los productos que caracterizan la cultura,<br>
    costumbres de Colombia, beneficiando en gran <br>
    parte a los artesanos independientes, que no <br>
    tienen acceso a las tecnologia digitales ni<br>
    tienen los recursos para adquirir lugares en <br>
    internet que ayuden a mostrar y comercializar <br>
    sus productos.<br>
    </p>
  </div>
</template>

<script>
export default {
  name: 'ComponentDescription',
  props: {
    tittleDescription: String
  }
}

</script>

<style>
.column-right{
   width: 600px;
   height: 450px;
   float:right;
}
.column-left{
   width: 450px;
   height: 450px;
   float:left;
}
</style>
