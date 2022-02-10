<template>
  <div id="app">
    <header-box :menuProps="menuItems" />
    <jumbotron-box />
    <first-section-box />
    <second-section-box />
    <third-section-box />
    <fourth-section-box />
    <fifth-section-box />
    <sixth-section-box />
    <seventh-section-box />
    <footer-box :footerProps="footerItems"/>
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
      menuItems: ["Home", "Apple", "Microsoft", "Android", "Forum", "Contact us"],
      footerItems: [
        {
          title: "popular topics",
          item1: "Nam a dolor voluptat massa auctor semper",
          item2: "Sed euismod nunc urna fermentum arcu dapibus fringilla",
          item3: "Cras lacinia tellus id mauris finibus lacus molestie",
          item4: "Curabitur a scelerisque ligula",
        },
        {
          title: "recent topic",
          item1: "Cras lacinia tellus id mauris finibus lacus molestie",
          item2: "Proin at ligula sagittis vestibulum nisi vitae",
          item3: "Sed nec metus at est tincidunt elementum",
          item4: "Nulla egestas nulla eu nulla suscipit molestie",
        },
        {
          title: "latest replies",
          item1: "Cras lacinia tellus id mauris finibus lacus molestie",
          item2: "Cras lacinia tellus id mauris finibus lacus molestie",
          item3: "Nulla egestas nulla eu nulla suscipit molestie",
          item4: "Mauris ac nibh quis eros sagittis lacinia a et dui",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
</style>
