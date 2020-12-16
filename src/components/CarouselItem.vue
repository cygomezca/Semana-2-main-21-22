<template>
    <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators">
            <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
            <li data-target="#carouselExampleCaptions" data-slide-to="3" class=""></li>
        </ol>
        <div class="carousel-inner">
            <div class="carousel-item active">
                
                <a href="../App.vue#services"><svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg"
                    preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: First slide"
                    src=../../public/img/services.jpg></svg></a>
                   <img src="../../public/img/services.jpg" alt="services">
                  <div class="carousel-caption d-none d-md-block">
                    
                    <h5 class="subtitulo "><a href="../App.vue#services">Servicios</a></h5>
                    <p class="contenido">Aqui sus mejores servicios de temporada </p>
                    
                </div>
            </div>
            <div class="carousel-item">
                
                <a href="../App.vue#news"><svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg"
                    preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: First slide"
                    src=../../public/img/noticias.jpg></svg></a>
                   <img src="../../public/img/noticias.jpg" alt="noticias">
                  <div class="carousel-caption d-none d-md-block">
                    
                    <h5 class="subtitulo "><a href="../App.vue#news">Noticias</a></h5>
                    <p class="contenido">Descubre las mejores noticias nacionales y del mundo solo aqui en tu canal de noticias</p>
                    
                </div>
            </div>
            <div class="carousel-item">
                <a href="../App.vue#members"><svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg"
                    preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: Second slide">
                    </svg>
                    <img src="../../public/img/equipo.jpg" ></a>
                <div class="carousel-caption d-none d-md-block">
                    <h5 class="subtitulo"><a href="../App.vue#members">Equipo desarrollador</a></h5>
                    <p class="contenido">Conoce nuestros miembros que logran desarrollar este proyecto</p>
                </div>
            </div>
            <div class="carousel-item">
                <a href="../App.vue#contacto"><svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg"
                    preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: Third slide">
                    </svg></a>
                  <title="contacto"> <img alt="contacto" src="../../public/img/contacto.jpg" >
                    <div class="carousel-caption d-none d-md-block">
                    <h5 class="subtitulo"><a href="../App.vue#contacto">Contacto</a></h5>
                    <p class="contenido">Quieres comunicarte con nosotros dar click aqui</p>
                    
                </div>
            </div>
        </div>
        <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
        </a>
    </div>
</template>

<script>
export default {
    name: "CarouselItem",
}
</script>