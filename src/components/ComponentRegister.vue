<template>
   <div class="column-inicio">
      <h4>INICIAR SESIÓN</h4><br>
      <form>
        <div class="mb-3">
          <label for="mail"
             class="form-label">
          Email address
          </label>
          <input type="email"
             class="form-control"
             id="mail"
             aria-describedby="emailHelp"
             placeholder="example@mail.com">
        </div>
        <div class="mb-3">
          <label for="pass"
             class="form-label">
          Password
          </label>
          <input type="password"
             class="form-control"
             id="pass"
             placeholder="********"
             maxlength="8">
        </div>
        <button type="button"
              class="btn btn-primary"
              data-bs-toggle="modal"
              data-bs-target="#ingreso">
        Ingresar
        </button>
          <div class="modal fade"
            id="ingreso"
            tabindex="-1"
            aria-hidden="true"
            v-if=" emailForm  === emailForm">
          <div class="modal-dialog">
           <div class="modal-content">
             <div class="modal-header">
              <button type="button"
                   class="btn-close"
                   data-bs-dismiss="modal"
                   aria-label="Close">
              </button>
             </div>
             <div class="modal-body">
              Bienvenid@ {{ name }} a Start.com
             </div>
           </div>
          </div>
          </div>
      </form>
   </div>
  <div class="column-register">
  <h4>REGISTRARSE</h4><br>
  <form>
      <div>
        <label class="form-label">Name</label>
        <input type="text"
               class="form-control"
               placeholder="First name"
               v-model="nameForm">
      </div><br>
      <div>
        <label class="form-label">Last Name</label>
        <input type="text"
               class="form-control"
               placeholder="Last name"
               v-model="lastnameForm">
      </div>
      <div>
        <label class="form-label">E-mail</label>
        <input type="email"
               class="form-control"
               placeholder="example@mail.com"
               aria-describedby="emailHelp"
               v-model="emailForm">
      </div>
      <div>
        <label class="form-label">Password</label>
        <input type="password"
               class="form-control"
               placeholder="********"
               v-model="passwordForm">
      </div><br>
      <button type="button"
              @click="ChangeInfo"
              class="btn btn-primary"
              data-bs-target="#register"
              data-bs-toggle="modal">
        Guardar
      </button>
      <div class="modal fade"
           id="register"
           tabindex="-1"
           aria-hidden="true">
          <div class="modal-dialog">
            <div class="modal-content">
              <div class="modal-header">
                <button type="button"
                        class="btn-close"
                        data-bs-dismiss="modal"
                        aria-label="Close">
                </button>
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
      type: String,
      require: true
    },
    lastname: {
      type: String,
      require: true
    },
    email: {
      type: String,
      require: true
    },
    password: {
      type: String,
      require: true
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
