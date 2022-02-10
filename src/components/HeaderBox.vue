<template>
  <header class="fixed-top">
    <div class="container">
      <div class="d-flex justify-content-between align-items-center py-2">
        <div>
          <img class="logo" :src="`/img${logoProps}`" alt="" />
        </div>
        <nav>
          <ul class="d-flex align-items-center">
            <li v-for="(item, index) in menuProps" :key="index">
              <a href="#">{{ item }}</a>
            </li>
            <li>
              <button class="text-uppercase fw-bold rounded">
                <a href="#">join us</a>
              </button>
            </li>

            <li>
              <i id="lens" class="fas fa-search"></i>
            </li>
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
