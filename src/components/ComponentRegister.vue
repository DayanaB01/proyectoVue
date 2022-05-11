<template>
  <div class="column-inicio">
  <h4>INICIAR SESIÓN</h4><br>
   <form>
     <div class="mb-3">
      <label for="exampleInputEmail1" class="form-label">Email address</label>
      <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="example@mail.com">
     </div>
     <div class="mb-3">
      <label for="exampleInputPassword1" class="form-label">Password</label>
      <input type="password" class="form-control" id="exampleInputPassword1" placeholder="********">
     </div>
     <button type="submit" class="btn btn-primary">Ingresar</button>
   </form>
  </div>
  <div class="column-register">
  <h4>REGISTRARSE</h4><br>
  <form>
      <div class="col">
        <label class="form-label">Name</label>
        <input type="text" class="form-control" placeholder="First name" aria-label="First name">
      </div><br>
      <div class="col">
        <label class="form-label">Last Name</label>
        <input type="text" class="form-control" placeholder="Last name" aria-label="Last name">
      </div>
      <div class="col">
        <label class="form-label">E-mail</label>
        <input type="email" class="form-control" placeholder="example@mail.com" aria-describedby="emailHelp">
      </div>
      <div class="col">
        <label class="form-label">Password</label>
        <input type="password" class="form-control" placeholder="********" aria-label="password">
      </div><br>
      <button type="button" class="btn btn-primary">Guardar</button>
  </form>
  </div>
</template>

<script>
export default {
  name: 'ComponentRegister'
}
</script>

<style>
  .column-inicio{
      float: left;
      width: 500px;
  }
  .column-register{
      width: 500px;
      float: right;
  }
  h4{
      text-align: center;
      font-family: cursive;
      color: black;
  }
</style>
