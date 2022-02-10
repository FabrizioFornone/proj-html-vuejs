<template>
  <div id="app">
    <header-box :menuProps="menu" />
    <jumbotron-box />
    <first-section-box />
    <second-section-box />
    <third-section-box />
    <fourth-section-box />
    <fifth-section-box />
    <sixth-section-box />
    <seventh-section-box />
    <footer-box />
  </div>
</template>

<script>
import HeaderBox from "./components/HeaderBox.vue";
import JumbotronBox from "./components/JumbotronBox.vue";
import FirstSectionBox from "./components/FistSectionBox.vue";
import SecondSectionBox from "./components/SecondSectionBox.vue";
import ThirdSectionBox from "./components/ThirdSectionBox.vue";
import FourthSectionBox from "./components/FourthSectionBox.vue";
import FifthSectionBox from "./components/FifthSectionBox.vue";
import SixthSectionBox from "./components/SixthSectionBox.vue";
import SeventhSectionBox from "./components/SeventhSectionBox.vue";
import FooterBox from "./components/FooterBox.vue";
export default {
  name: "App",
  components: {
    HeaderBox,
    JumbotronBox,
    FirstSectionBox,
    SecondSectionBox,
    ThirdSectionBox,
    FourthSectionBox,
    FifthSectionBox,
    SixthSectionBox,
    SeventhSectionBox,
    FooterBox,
  },
  data() {
    return {
      menu: ["Home", "Apple", "Microsoft", "Android", "Forum", "Contact us"],
    };
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
</style>
