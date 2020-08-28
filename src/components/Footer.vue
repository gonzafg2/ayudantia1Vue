<template>
  <div class="footer">
    <h2>Directivas de Vue</h2>
    <div class="frutas">
      <input type="text" />
      <button class="frutas__btn">Agregar fruta</button>
    </div>
  </div>
  
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      frutas: [],
      fruta: ""
    }
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
    }
  }
}
</style>