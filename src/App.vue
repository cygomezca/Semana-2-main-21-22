<template>
  <div id="app">

    <!-- carousel -->
    
    <carousel-item></carousel-item>
    <!-- Services -->
    <div class="container-fluid p-3 my-3 " id="services">
        <div class="container-fluid text-center bg-dark text-light">
              <h2 class="section-heading text-uppercase">Servicios</h2>
          </div>
    </div>
    <services-section></services-section>

    <!-- news -->
      <div class="container-fluid p-3 my-3 bg-info " id="news">
          <div class="container-fluid text-center bg-dark text-light">
              <h2 class="section-heading text-uppercase">Noticias</h2>
          </div>          
          <news-section></news-section>    
      </div>

    <!-- Container Members -->
      <div class="container-fluid p-3 my-3 " id="members">
        <div class="container-fluid text-center bg-dark text-light">
              <h2 class="section-heading text-uppercase">Equipo</h2>
          </div>
        <div class="row justify-content-center mb-5">
          <div class="col mt-5" v-for="(miembro, index) of Team" :key="index"> 
            <team-card :member="miembro"> </team-card>
          </div> 
        </div>
     </div>    

    <!-- Footer -->
    <div  class="page-footer bg-secondary text-white pt-4" id="contacto">
      <div class="container-fluid text-center text-md-left">

        <!-- Grid row -->
        <div class="row">

            <!-- Grid column -->
            <div class="col-md-6 mt-md-0 mt-3">

                <!-- Content -->
                <h5 class="text-uppercase font-weight-bold">Informacion</h5>
                <p>Este sitio fue creado como reto sprint 1 ciclo 3 con la Universidad UTP con el fin de implementar diferentes herramientas para crear paginas web </p>
                <h5 class="text-uppercase font-weight-bold"><a href="https://github.com/cygomezca/Semana-2-main-21-22.git" target="_blank">Repositorio github</a></h5>     
            </div>
            <!-- Grid column -->

            <hr class="clearfix w-100 d-md-none pb-3">
                    
            <!-- Grid column -->
            <div class="col-md-6 mb-md-0 mb-3">
              <h5 class="text-uppercase font-weight-bold">Contactos</h5>
            <div class="row justify-content-center mb-6">
            <div class="col mt-6" v-for="(miembro2, index) of Team" :key="index"> 
            <footer-section :footer="miembro2"></footer-section>
            </div> 
            </div>
          </div>
        </div>
          <!-- Grid row -->
        </div>
      </div>
    <!-- Footer Text -->

    <!-- Copyright -->
    <div class="footer-copyright text-center py-1 bg-white">© 2020 Copyright: DAD
    </div>    
       
  </div>
</template>

<script>


import CarouselItem from './components/CarouselItem.vue'
import ServicesSection from './components/ServicesSection.vue'
import NewsSection from "./components/NewsSection.vue"
import TeamCard from './components/TeamCard.vue'
import FooterSection from './components/FooterSection.vue'

export default {
  name: 'App',
  components: {
    CarouselItem,
    ServicesSection,
    NewsSection,
    TeamCard,
    FooterSection,
    
  },
  data(){
    return{
    Team:[
        {
          codigo: 1,
          nombre:'Carmen Yisella Gomez Castillo',
          contacto: '3104510576',
          correo: 'yiscan55@gmail.com',
          descripcion:'Ingeniera de petróleos, docente en el área de matemáticas, networker, actualmente estudio una especialización en pedagogía en la UNAD, programación con MinTic y guianza turística con el Sena. Me gusta leer, viajar, aprender cosas nuevas y ver documentales.', 
          rol: 'Docente',
          image: 'https://imgur.com/xmL9c29.jpg'
        },

        {
          codigo: 2,
          nombre:"David Barrios Rodríguez",
          descripcion:'23 años, Ingeniero Químico.',
          contacto: '3024459660', 
          correo: 'davidbar22@hotmail.com',
          rol: 'Quimico',
          image: 'https://imgur.com/SlH1buC.jpg'
        },

        {
          codigo: 3,
          nombre:'Maritza Moreno Montejo',
          descripcion:'Técnico en Sistemas, Cosmetología Esteticista, 43 años',
          contacto: '3234492471', 
          correo: 'maritzamontejo1234 2016@',
          rol: 'Estilista',
          image: 'https://imgur.com/3UcCcsb.jpg'
        },

        {
            codigo: 4,
            nombre:'Jorrique Durán Ayala',
            descripcion:'Estudiante de Ing. Electrónica. Desarrollador en formación. Músico en los ratos libres',
            contacto: '+584147417189',
            correo:'jorriqueduran@gmail.com',
            rol: 'Desarrollador',
            image: 'https://imgur.com/w66hONq.jpg'
        },

        {
          codigo: 5,
          nombre:'Lizeth Catherine Ortiz',
          descripcion:'Estudiante de Ciencias de la Computación. Me gusta la música, leer y practico danza árabe.',
          contacto: '3197623800', 
          correo: 'liortiz@unal.edu.co',
          rol: 'Cientifica',
          image: 'https://imgur.com/wqIAAkZ.jpg'
        },

        {
          codigo: 6,
          nombre:'Juan Camilo Castro Yara',
          descripcion:'Ingeniero en un 98%, me gusta tocar guitarra, jugar futbol de hecho estuve en la liga de bogota casi me ficha el cucuta, practicar boxeo estuve en algunos torneos del IDRD, me gusta montar bicicleta comer cosas nuevas en un futuro viajar por el mundo, coprarme el carro de mis sueños y ser feliz.',
          contacto: '3133932800', 
          correo: 'juanca-castro@hotmail.com',
          rol: 'Ingeniero en Sistemas',
          image: 'https://imgur.com/gN5WAKF.jpg'
        }
      ]
    }
  }
}
</script>
