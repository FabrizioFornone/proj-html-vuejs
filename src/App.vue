<template>
  <div id="app">
    <header-box :menuProps="menuItems" logoProps="/logo-2x.png" />
    <jumbotron-box />
    <heading-text-box />
    <first-item-row-box :latestNewsProps="latestNews" />
    <featured-article-box />
    <second-item-row-box :latestNews2Props="latestNews2" />
    <tutorial-and-guide-box :tutorialAndGuideProps="tutorialAndGuide" />
    <forum-sections-box :iconsProps="icons" />
    <community-and-subscribe-box />
    <footer-box :footerProps="footerItems" />
  </div>
</template>

<script>
import HeaderBox from "./components/HeaderBox.vue";
import JumbotronBox from "./components/JumbotronBox.vue";
import HeadingTextBox from "./components/HeadingTextBox.vue";
import FirstItemRowBox from "./components/FirstItemRowBox.vue";
import FeaturedArticleBox from "./components/FeaturedArticleBox.vue";
import SecondItemRowBox from "./components/SecondItemRowBox.vue";
import TutorialAndGuideBox from "./components/TutorialAndGuideBox.vue";
import ForumSectionsBox from "./components/ForumSectionsBox.vue";
import CommunityAndSubscribeBox from "./components/CommunityAndSubscribeBox.vue";
import FooterBox from "./components/FooterBox.vue";
export default {
  name: "App",
  components: {
    HeaderBox,
    JumbotronBox,
    HeadingTextBox,
    FirstItemRowBox,
    FeaturedArticleBox,
    SecondItemRowBox,
    TutorialAndGuideBox,
    ForumSectionsBox,
    CommunityAndSubscribeBox,
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
      icons: [
        {
          name: "file-alt",
          prefix: "fa-",
          family: "fas",
        },
        {
          name: "apple",
          prefix: "fa-",
          family: "fab",
        },
        {
          name: "windows",
          prefix: "fa-",
          family: "fab",
        },
        {
          name: "android",
          prefix: "fa-",
          family: "fab",
        },
        {
          name: "coffee",
          prefix: "fa-",
          family: "fas",
        },
        {
          name: "cubes",
          prefix: "fa-",
          family: "fas",
        },
        {
          name: "laptop",
          prefix: "fa-",
          family: "fas",
        },
        {
          name: "wrench",
          prefix: "fa-",
          family: "fas",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
</style>
