<template>
  <div id="app">
    <page-header></page-header>
    <section-api> </section-api>
    
    <div class="container-fluid">
      <div class="row">
        <div class="col mt-5" v-for="(item, index) of team " :key="index">
        <team-card v-bind:member= "item"></team-card>
      </div>
    </div>
    </div>
  </div>
</template>

<script>
import PageHeader from "./components/PageHeader.vue";
import SectionApi from "./components/SectionApi";
import TeamCard from './components/TeamCard.vue';
const imgLink = require('../public/images/ndml.jpg');
const imgLink1 = require('../public/images/cyms.jpg');
const imgLink2 = require('../public/images/yss.jpg');
const imgLink3 = require('../public/images/jcba.jpg');
const imgLink4 = require('../public/images/lfm.jpg');
export default {
  name: "App",
  components: {
    PageHeader,
    SectionApi,
    TeamCard
  },
  data (){
    return{
      team: [
        {
          codigo: 1,
          nombre: "Neiry Dayan Martinez Lara",
          descripcion: "Ingeniera Biomédica de la Universidad Manuela Beltran               Pasatiempos: Jugar fútbol y ver series.",
          rol: "Desarrollador Frontend",
          image: imgLink
        },
        {
          codigo: 2,
          nombre: "Cristian Yesid Marin ",
          descripcion: " Ingeniero Electronico de la Universidad Central                         Pasatiempos: Practicar deportes como el futbol de salón y el baloncesto, ir al cine con su familia.",
          rol: "Desarrollador backend",
          image: imgLink1
        },
        {
          codigo: 3,
          nombre: "Yesenia Sánchez Sánchez",
          descripcion: "Administradora de empresas de la Universidad del Valle            Pasatiempos: Viajar.",
          rol: "Desarrollador backend",
          image: imgLink2
        },
        {
          codigo: 4,
          nombre: "Juan Camilo Bazurto Arias",
          descripcion: "Estudiante de Ingenieria en Sistemas de la Escuela Colombiana de Ingenieria Julio Garavito, Pasatiempos: Leer, hacer ejercicio y practicar futbol.",
          rol: "Desarrollador Frontend",
          image: imgLink3
        },
        {
          codigo: 5,
          nombre: "Luis Felipe Martínez",
          descripcion: "Ingeniero en Sistemas de la Universidad Autónoma del Caribe, Pasatiempos: jugar voleyball, trotar, salir a comer, leer manga,ver anime y visitar a mi novia",
          rol: "Scrum Master",
          image: imgLink4
        }
      ]
    }
  }
};

</script>


