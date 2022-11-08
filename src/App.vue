<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppBlueBar from "./components/AppBlueBar.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: {
    AppHeader,
    AppMain,
    AppBlueBar,
    AppFooter
  }
}
</script>


<template>

  <header>
    <AppHeader />
  </header>

  <main>
    <AppMain />
    <AppBlueBar />
  </main>

  <footer>
    <AppFooter />
  </footer>

</template>


<style lang="scss">
@use "./styles/general.scss" as *;

header {
  max-width: 1200px;
  margin: auto;
}

main {
  background-color: black;
  margin: auto;
}

body {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
