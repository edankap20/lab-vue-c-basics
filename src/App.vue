<template>
  <navbar></navbar>
  <h1>El resultado de la operación 2 + 2 es: {{ 2 + 2 }} </h1>
  <h1>{{ textoGenerado }}</h1>
  <BackgroundColorChanger></BackgroundColorChanger>
  <Footer></Footer>
</template>


<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
import BackgroundColorChanger from './components/BackgroundColorChanger.vue'
export default {
  name: 'App',
  data() {
    return {
      nombre: "Johan",
      apellido: "Uibe",
      edad: 33,
    }
  },
  computed: {
    textoGenerado(){
      return `Hola, mi nombre es ${this.nombre} ${this.apellido} y tengo ${this.edad} años.`
    }
  },
  components: {
    Navbar,
    Footer,
    BackgroundColorChanger
}
}
</script>


<style scoped>
</style>
