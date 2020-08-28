<template>
  <div class="navbar">
    <section class="section1">
      <ul>
        <li></li>
        <li></li>
        <li></li>
      </ul>
      <MiniNavBar />
    </section>
  </div>
</template>

<script>
import MiniNavBar from "./MiniNavBar";

export default {
  name: "NavBar",
  components: {
    MiniNavBar,
  },
}
</script>

<style lang="scss" scoped>

</style>