<template>
  <div id="app">
    <header-box :menuProps="menuItems" logoProps="/logo-2x.png" />
    <jumbotron-box />
    <first-section-box />
    <second-section-box :latestNewsProps="latestNews" />
    <third-section-box />
    <fourth-section-box :latestNews2Props="latestNews2" />
    <fifth-section-box :tutorialAndGuideProps="tutorialAndGuide" />
    <sixth-section-box />
    <seventh-section-box />
    <footer-box :footerProps="footerItems" />
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
      menuItems: [
        "Home",
        "Apple",
        "Microsoft",
        "Android",
        "Forum",
        "Contact us",
      ],
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
      latestNews: [
        {
          img: "/smartphone1.jpg",
          title: "Morbi vitae dui euismod vuluptate sollicitudin",
          subtitle: "October 11th, 205 |",
          comments: "2 comments",
          paragraph:
            "Donec finibus sit aemet orci eget ultricies. Praesent posuere ante ut erat fringilla, stibulum placerat metus mattis. Aenean dictum vitae nisl",
        },
        {
          img: "/smartphone2.jpg",
          title: "Vivamus pellenteque, felis quis varius",
          subtitle: "October 11th, 205 |",
          comments: "Comments Off",
          paragraph:
            "Donec finibus sit aemet orci eget ultricies. Praesent posuere ante ut erat fringilla, stibulum placerat metus mattis. Aenean dictum vitae nisl",
        },
        {
          img: "/smartwatch.jpg",
          title: "Donec ornare pretium eget scelisque justo",
          subtitle: "October 11th, 205 |",
          comments: "Comments Off",
          paragraph:
            "Donec finibus sit aemet orci eget ultricies. Praesent posuere ante ut erat fringilla, stibulum placerat metus mattis. Aenean dictum vitae nisl",
        },
      ],
      latestNews2: [
        {
          img: "/tablet1.jpg",
          title: "Morbi vitae dui euismod vuluptate sollicitudin",
          subtitle: "October 11th, 205 |",
          comments: "2 comments",
          paragraph:
            "Donec finibus sit aemet orci eget ultricies. Praesent posuere ante ut erat fringilla, stibulum placerat metus mattis. Aenean dictum vitae nisl",
        },
        {
          img: "/camera1.jpg",
          title: "Vivamus pellenteque, felis quis varius",
          subtitle: "October 11th, 205 |",
          comments: "Comments Off",
          paragraph:
            "Donec finibus sit aemet orci eget ultricies. Praesent posuere ante ut erat fringilla, stibulum placerat metus mattis. Aenean dictum vitae nisl",
        },
        {
          img: "/desktop1.jpg",
          title: "Donec ornare pretium eget scelisque justo",
          subtitle: "October 11th, 205 |",
          comments: "Comments Off",
          paragraph:
            "Donec finibus sit aemet orci eget ultricies. Praesent posuere ante ut erat fringilla, stibulum placerat metus mattis. Aenean dictum vitae nisl",
        },
      ],
      tutorialAndGuide: [
        {
          img: "/tablet1.jpg",
          title: "Morbi vitae dui euismod vuluptate sollicitudin",
          subtitle: "October 11th, 205 |",
          comments: "2 comments",
          paragraph:
            "Donec finibus sit aemet orci eget ultricies. Praesent posuere ante ut erat fringilla, stibulum placerat metus mattis. Aenean dictum vitae nisl",
        },
        {
          img: "/camera1.jpg",
          title: "Vivamus pellenteque, felis quis varius",
          subtitle: "October 11th, 205 |",
          comments: "Comments Off",
          paragraph:
            "Donec finibus sit aemet orci eget ultricies. Praesent posuere ante ut erat fringilla, stibulum placerat metus mattis. Aenean dictum vitae nisl",
        },
        {
          img: "/desktop1.jpg",
          title: "Donec ornare pretium eget scelisque justo",
          subtitle: "October 11th, 205 |",
          comments: "Comments Off",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
</style>
