<template>
<div class="d-flex justify-content-center align-items-center  row mt-md-5 mt-sm-5 mt-xs-5">
    
    <div class=" col-lg-6 col-xs-12 stretch" v-for="(item,index) of noticias" :key="index">
                <div class="d-flex justify-content-center align-items-center bg-light" >
    
                    <div class="p-3">
                        <img :src="item.urlToImage" height="250" width="250">
                    </div>
    
                    <div class="p-2">
                        <h3>{{item.title}}</h3>
                        <p>
                            {{item.description}}
                        </p>
                    </div>
    
                </div>
                <div class="d-flex container-fluid align-items-center  justify-content-end pb-2 mt-n2 bg-dark text-white">
                    <a class="align-items-center" :href='item.url' >
                        <button type="button" class=" btn btn-info">Abrir</button>    
                    </a>
                </div>
            </div>
 </div>
</template>

<script>
import axios from "axios"
export default {
    name:"NewsSection",
    data(){
        return{
            noticias:null,}
    },
    mounted(){
        axios
        .get('http://newsapi.org/v2/top-headlines?country=co&category=science&apiKey=f73e9b4ac6ed446eaa8e6a3a14c72994')
        .then( response => (this.noticias = response.data.articles.slice(0,4)))
        // console.log(this.peliculas)

    },
}
</script>