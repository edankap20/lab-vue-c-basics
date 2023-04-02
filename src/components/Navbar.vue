<template lang="">
    <div>
        <h2 v-show="mostrarNavbar">Navbar</h2>
        <button @click="toggleMostrarMensaje">Mostrar/Ocultar mensaje</button>
    </div>
</template>

<script>
export default {
    data(){
        return {
            mostrarNavbar: true,
        }
    },
    methods: {
        toggleMostrarMensaje (){
            this.mostrarNavbar = !this.mostrarNavbar
        }
    }
}
</script>

<style lang=""> 
</style>