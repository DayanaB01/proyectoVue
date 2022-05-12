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
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModala">
  Ingresar
</button>
<div class="modal fade" id="exampleModala" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        Bienvenido {{ nameData }} a Start.com
      </div>
    </div>
  </div>
</div>

   </form>
  </div>
  <div class="column-register">
  <h4>REGISTRARSE</h4><br>
  <form>
      <div class="col">
        <label class="form-label">Name</label>
        <input type="text" class="form-control" placeholder="First name" aria-label="First name" v-model="nameData">
      </div><br>
      <div class="col">
        <label class="form-label">Last Name</label>
        <input type="text" class="form-control" placeholder="Last name" aria-label="Last name" v-model="lastnameData">
      </div>
      <div class="col">
        <label class="form-label">E-mail</label>
        <input type="email" class="form-control" placeholder="example@mail.com" aria-describedby="emailHelp" v-model="emailData">
      </div>
      <div class="col">
        <label class="form-label">Password</label>
        <input type="password" class="form-control" placeholder="********" aria-label="password" v-model="passwordData">
      </div><br>
      <button type="button" class="btn btn-primary" @click="saveInfo">Guardar</button>
  </form>
  </div>
</template>

<script>
export default {
  name: 'ComponentRegister',
  beforeMount () {
    this.nameData = this.name
    this.lastnameData = this.lastname
    this.emailData = this.email
    this.passwordData = this.password
  },
  data () {
    return {
      nameData: '',
      lastnameData: '',
      emailData: '',
      passwordData: ''
    }
  },
  props: {
    name: {
      type: String,
      required: true
    },
    lastname: {
      type: String,
      required: true
    },
    email: {
      type: String,
      required: true
    },
    password: {
      type: String,
      required: true
    }
  },
  methods: {
    saveInfo () {
      this.$emit('getData', {
        name: this.nameData,
        lastname: this.lastnameData,
        email: this.emailData,
        password: this.password
      })
    }
  }
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
