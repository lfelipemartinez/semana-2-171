<template>
  <footer class="page-footer bg-info text-white pt-4">
    <div class="container-fluid text-center text-md-left">
      <div class="row">
        <div class="col-md-5 mt-md-0 mt-3">
          <h5 class="text-uppercase font-weight-bold">Acerca de nosotros</h5>
          <p>
            <br>Biomedical S.A.S Es una empresa dedicada al servicio y mejoramiento
            de procesos internos y externos en gestion hospitalaria, cronogramas
            de mantenimiento y desarrrollo de sofware enfocado a garantizar
            altos estandares de calidad en salud, tanto para el prestador de
            salud como para sus usuarios.<br><br>
            TELEFONO: 6989898<br>
            CORREO: biom_solutions@biomedical.net.co
          </p>

        </div>

        <hr class="clearfix w-100 d-md-none pb-3" />

        <div class="col-md-6 mb-md-0 mb-4">
          <h5 class="text-uppercase font-weight-bold">
            Contactese para mayor informacion
          </h5>
          <div class="form-group">
            <input type="text" placeholder="Nombre" class="form-control mt-4" v-model="nombre"/>
            <input
              type="email"
              placeholder="Correo"
              class="form-control mt-3"
              v-model="correo"
            />
            <div class="form-group">
              <textarea class="form-control mt-3" rows="5" placeholder="Mensaje" v-model="mensaje"></textarea>
            </div>
            <button class="btn btn-primary" v-on:click="enviar">Enviar</button>
          </div>
        </div>
      </div>
    </div>

    <div class="footer-copyright text-center py-1 bg-dark">
      BIOMEDICAL™
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data(){
      return{
          nombre: '',
          correo: '',
          mensaje: ''
      }
  },
  methods:{
      enviar(){
          this.nombre = '';
          this.correo = '';
          this.mensaje = '';
      }
  }
  
};
</script>

<style scoped></styles>