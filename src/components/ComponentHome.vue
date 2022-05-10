<template>
 <div class="column-start">
  <div class="card" style="width: 18rem;">
    <img src="@/assets/manillas.jpg" class="card-img-top" alt="manillas">
    <div class="card-body">
     <h5 class="card-title">Card title</h5>
     <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
     <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
  </div>
 </div>
 <div class="column-center">
  <div class="card" style="width: 18rem;">
    <img src="@/assets/manillas.jpg" class="card-img-top" alt="manillas">
    <div class="card-body">
     <h5 class="card-title">Card title</h5>
     <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
     <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
  </div>
 </div>
 <div class="column-end">
  <div class="card" style="width: 18rem;">
    <img src="@/assets/manillas.jpg" class="card-img-top" alt="manillas">
    <div class="card-body">
     <h5 class="card-title">Card title</h5>
     <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
     <a href="#" class="btn btn-primary">Go somewhere</a>
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
    float:inline-start;
    width: 300px;
  }
   .column-end{
    float:right;
    width: 300px;
  }
</style>
