<template>
  <div class="footer">
    <h2>Directivas de Vue</h2>
    <div class="frutas">
      <!-- Directivas son atributossssss!!!!!!! -->
      <input v-model="fruta" type="text" />
      <!-- Actualiza en tiempo real el valor de un estado (variable) -->
      <button class="frutas__btn">Agregar fruta</button>
      <!-- Interpolación de variables -->
      {{ fruta }}

      <!-- V-FOR -->
      <!-- Deben llevar un identificatorio único, como se lo paso? con el atributo :key="index" e index es el índice de cada elemento
      dentro del arreglo -->
      <section class="lista">
        <p v-for="(item, indice) in frutas" :key="indice">
          {{ item }}
        </p>
      </section>

      <!-- V-IF -->
      <!-- V-ELSE-IF -->
      <!-- V-ELSE -->
      <!-- V-SHOW -->
      <!-- V-ON:CLICK -->
      <Vivi />
      <Naty />
      <Dani />
    </div>
  </div>

</template>

<script>
import Vivi from './Viviana'
import Naty from './Natalia'
import Dani from './dani'

export default {
  name: "Footer",
  data() {
    return {
      frutas: ["Manzana", "Limón", "Pera"],
      fruta: ""
    }
  },
  components: {
    Vivi,
    Naty,
    Dani
  }
}
</script>

<style lang="scss" scoped>
.footer {
  color: red;
  .frutas {
    color: blue;
    &__btn {
      color: green;
      background-color: #fff;
      border: 1px solid #000;
      margin-left: 10px;
      padding: 5px;
      border-radius: 5px;
    }
  }
}
</style>