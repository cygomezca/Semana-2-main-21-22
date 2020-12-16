<template>
    <!-- services -->
<div class="container-fluid">
        <div class="row justify-content-center mb-5">
            <div class="col-sm-6 col-xs-12 col-lg-4 mt-5">
            
                <div class="card bg-light">
                        <div class="d-flex justify-content-center p-2">
                                <img :src="'https://i.imgur.com/fWpAjvk.jpg'" alt="Imagen de Mabel Amber en Pixabay" height="200" width="200">
                        </div>
                    <div class="card-body">
                        <h5 class="card-title content-center" align="center"> Horóscopo </h5>
                        <p class="card-text" align="center"> Conoce qué te depara tu futuro con tu carta astral, clic en el siguiente enlace para más información. </p>
                        <a href="https://www.univision.com/temas/horoscopo-diario" target="_blank" rel="noopener noreferrer" class="btn btn-primary"
                        > Conoce tu tarot aquí </a>
                    </div>
                </div>
            
            </div>
            <div class="col-sm-6 col-xs-12 col-lg-4 mt-5">
                <div class="card bg-light">
                    <div class="d-flex justify-content-center p-2">
                        <img :src="'https://i.imgur.com/7m2rlEp.jpg'" alt="Imagen de Eduardo Saint Jean en Pixabay " height="200" width="400">  
                    </div>
                    <div class="card-body">
                        <h5 class="card-title" align="center"> Entretenimiento </h5>
                        <p class="card-text" align="center"> ¿No tienes nada qué hacer? Ingresa acá y encuentra los mejores juegos para pasar el tiempo </p>
                        <a href="https://www.juegos.com/" class="btn btn-primary" target="_blank" rel="noopener noreferrer"
                        > Juegos aquí </a>
                    </div>
                </div>
            </div>
            <div class="col-sm-6 col-xs-12 col-lg-4 mt-5">
                    <div class="card bg-light">
                            <div class="d-flex justify-content-center p-2">
                                    <img :src="'https://i.imgur.com/0Ja9ixy.jpg'" alt="Imagen de Bruno Marques Designer en Pixabay" height="200" width="200">  
                                </div>
                            <div class="card-body">
                                <h5 class="card-title"> Página de domicilios </h5>
                                <p class="card-text"> ¿Con hambre? Pide con nosotros el desayuno, el almuerzo y la cena, ¡o incluso el mercado! </p>
                                <a href="https://domicilios.com/" class="btn btn-primary" target="_blank" rel="noopener noreferrer"
                                > Pide aquí </a>
                            </div>
                        </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name: 'ServicesSection'
}
</script>