<template>       
<div class="card text-black badge badge-secondary">       
    <div class="card-footer">
        <h7 class="card-title">{{ footer.nombre }}</h7>
        <br>
        <small class="text"> Contacto: {{ footer.contacto}} </small>
        <br>
        <small class="text"> Correo: {{ footer.correo}} </small>           
    </div>
</div>
</template>

<script>
    export default {
        name: "FooterSection",
        props: ['footer']
    }
</script>

<style scoped>

</style>