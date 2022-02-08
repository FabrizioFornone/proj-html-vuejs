<template>
  <div id="app">
    <header-box />
    <jumbotron-box />
    <first-section-box />
  </div>
</template>

<script>
import HeaderBox from "./components/HeaderBox.vue";
import JumbotronBox from "./components/JumbotronBox.vue";
import FirstSectionBox from "./components/FistSectionBox.vue";
export default {
  name: "App",
  components: { HeaderBox, JumbotronBox, FirstSectionBox },
};
</script>

<style lang="scss">
@import "./style/main.scss";
</style>
