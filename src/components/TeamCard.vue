<template>
    <div class="card-text-white bg-dark">
        <div class="d-flex justify-content-center p-2">
            <img v-bind:src= "member.image" alt="fotografia del miembro" width="200px" height="200px">
        </div>
    <div>
        <h2 class="miembro__nombre">{{ member.nombre }}</h2>
        <p class="card-text text-center text-white">{{ member.descripcion }}</p>
        <p class="card-text text-center text-white"><span> Rol: </span> {{ member.rol}}<p>
        <p class="card-text text-center text-white"><span> Codigo: </span> {{ member.codigo}}<p>
        </p>
                
    </div>
    </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: ["member"]
    }
</script>

<style scoped>

</style>
