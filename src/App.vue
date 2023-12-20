<script>
import CleanHeader from "./components/CleanHeader.vue"
export default {
  name: "App",
  components: { CleanHeader },
};
</script>

<template>
  <div id="app">
    <header>
      <CleanHeader />
    </header>
    <main></main>
    <footer></footer>
  </div>
</template>

<style lang="scss">
@use "./assets/style.scss" as *;
</style>
