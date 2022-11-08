<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";

export default {
  components: {
    AppHeader,
    AppMain
  }
}
</script>


<template>

  <header>
    <AppHeader />
  </header>

</template>


<style lang="scss" scoped>
@use "./styles/general.scss" as *;

header {
  max-width: 1200px;
  margin: auto;
}
</style>
