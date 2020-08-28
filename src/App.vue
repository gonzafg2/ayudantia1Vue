<!-- SIEMPRE DEBE IR CÓDIGO HTML DENTRO DE TEMPLATE!!!!! -->
<template>
  <div id="app">
    <!-- 3° Paso: Invocarlo!!!! Cómo? A través de una etiqueta HTML -->
    <NavBar></NavBar>
    <Footer />
  </div>
  <!-- TEMPLATE SÓLO ACEPTA UNA ETIQUETA!!! -->
  <!-- <div class="dos"></div>  -->
</template>

<script>
// 1° Paso: Importar componente!!!
import NavBar from "./components/Navbar"
import Footer from "./components/Footer"

export default {
  name: 'App',
  // 2° Paso: Incluirlo dentro de la propiedad "components".
  components: {
    NavBar,
    Footer
  }
}
</script>

<style lang="scss">
// Existen dos sintaxis de sass:

// 1° Extension .sass
// .miClase
//   color: red

// 2° Extension .scss
// Completamente compatible con css!!!
.miClase {
  color: red
}

</style>

<style scoped>
/* Se pueden agregar más de una etiqueta style */

/* La palabra reservada "scoped" sirve para SÓLO aplicar estilos a este componente !!! */
.miClase2 {
  color: black;
}
</style>
