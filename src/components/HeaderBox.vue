<template>
  <header class="fixed-top">
    <div class="container">
      <div class="d-flex justify-content-between align-items-center py-2">
        <div>
          <a href="#">
            <img class="logo" :src="`/img${logoProps}`" alt="" />
          </a>
        </div>
        <nav class="d-flex align-items-center">
          <ul class="d-flex align-items-center">
            <li
              v-for="(item, index) in menuProps"
              :key="index"
              class="d-flex align-items-center"
            >
              <a class="d-flex align-items-center" href="#">{{ item }}</a>
            </li>
            <button class="text-uppercase fw-bold rounded btn">
              <a href="#">join us</a>
            </button>
            <i id="lens" class="fas fa-search px-4"></i>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  props: {
    logoProps: String,
    menuProps: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/headerStyle.scss";
</style>
