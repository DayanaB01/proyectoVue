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
            Bienvenid@ a Start.com
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
        <input type="text" class="form-control" placeholder="First name" aria-label="First name" v-model="nameForm">
      </div><br>
      <div class="col">
        <label class="form-label">Last Name</label>
        <input type="text" class="form-control" placeholder="Last name" aria-label="Last name" v-model="lastnameForm">
      </div>
      <div class="col">
        <label class="form-label">E-mail</label>
        <input type="email" class="form-control" placeholder="example@mail.com" aria-describedby="emailHelp" v-model="emailForm">
      </div>
      <div class="col">
        <label class="form-label">Password</label>
        <input type="password" class="form-control" placeholder="********" aria-label="password" v-model="passwordForm">
      </div><br>
      <button type="button" class="btn btn-primary" data-bs-target="#exampleModa" data-bs-toggle="modal">Guardar</button>
      <div class="modal fade" id="exampleModa" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog">
         <div class="modal-content">
          <div class="modal-header">
           <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close" @click="ChangeInfo"></button>
          </div>
          <div class="modal-body">
            {{ name }} {{ lastname }} ya estas registrad@ en Start.com
          </div>
         </div>
        </div>
       </div>
  </form>
  </div>
</template>

<script>
export default {
  name: 'ComponentRegister',
  data () {
    return {
      nameForm: '',
      lastnameForm: '',
      emailForm: '',
      passwordForm: ''
    }
  },
  props: {
    name: {
      type: String
    },
    lastname: {
      type: String
    },
    email: {
      type: String
    },
    password: {
      type: String
    }
  },
  methods: {
    ChangeInfo () {
      this.$emit('getForm', {
        name: this.nameForm,
        lastname: this.lastnameForm,
        email: this.emailForm,
        password: this.passwordForm
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
