
<template>
    <div>
        <div class="card text-white bg-dark">
            <div class="d-flex justify-content-center p-2">
                <img :src="member.image" alt="foto del equipo" height="150" width="150">
            </div>
            <div class="card-body">
                <h5 class="card-title">{{ member.nombre }}</h5>
                <p class="card-text"> {{ member.descripcion}} </p>
            </div>
            <div class="card-footer">
                <small class="text-muted"> Rol: {{ member.rol}} </small>
                <br>
                <small class="text-muted"> Codigo: {{ member.codigo}} </small>
                <br>
                <small class="text-muted"> Contacto: {{ member.contacto}} </small>
                <br>
                <small class="text-muted"> Correo: {{ member.correo}} </small>
            </div>
        </div>
    </div>

</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>