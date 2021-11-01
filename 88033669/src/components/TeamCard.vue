<template>
        
        <div class="card text-white bg-dark">
            <div class="d-flex justify-content-center p-2">
                <img :src="member.imagen" alt="Fotografía del equipo" >
            </div>
            <div class="card-body">
                <p class="card-text"><span class="amarillo"> Código: </span> <span class="rojo">{{ member.codigo }}</span>,</p>
                <p class="card-text"><span class="amarillo">Nombre: </span> <span class="verde"> {{member.nombre }}</span>,</p>
                <p class="card-text"><span class="amarillo">Descripción: </span> <span class="verde">{{ member.descripcion }}</span>,</p>
                <p class="card-text"><span class="amarillo">Rol: </span> <span class="verde"> {{member.rol }}</span>,</p>
                <p class="card-text"><span class="amarillo">Imagen: </span> <span class="verde">{{ member.imgagen }}</span></p>
            </div>
            <div class="card-footer">
                <small class="text-muted">Last updated 3 mins ago</small>
            </div>
            <pre>
            </pre>
        </div>
    
</template>

<script>
// Estamos recibiendo el objeto miembro por props correctamente pero las pruebas nos siguen saliendo mal
// Al parecer nos estamos olvidando de algo
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>
