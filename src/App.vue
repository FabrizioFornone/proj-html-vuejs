<template>
  <div id="app">
    <header-box />
    <jumbotron-box />
    <first-section-box />
    <second-section-box />
  </div>
</template>

<script>
import HeaderBox from "./components/HeaderBox.vue";
import JumbotronBox from "./components/JumbotronBox.vue";
import FirstSectionBox from "./components/FistSectionBox.vue";
import SecondSectionBox from "./components/SecondSectionBox.vue";
export default {
  name: "App",
  components: { HeaderBox, JumbotronBox, FirstSectionBox, SecondSectionBox },
};
</script>

<style lang="scss">
@import "./style/main.scss";
</style>
