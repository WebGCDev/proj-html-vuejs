<script>
import CleanHeader from "./components/CleanHeader.vue"
import CleanMain from "./components/CleanMain.vue";
export default {
  name: "App",
  components: { CleanHeader, CleanMain },
};
</script>

<template>
  <div id="app">
    <header>
      <CleanHeader />
    </header>
    <main>
      <CleanMain />
    </main>
    <footer></footer>
  </div>
</template>

<style lang="scss">
@use "./assets/style.scss" as *;
</style>
