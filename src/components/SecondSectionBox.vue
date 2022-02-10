<template>
  <section>
    <div class="container pt-5 my-3">
      <div class="text-center">
        <h5 class="text-uppercase">phasellus eget metus</h5>
        <h2 class="fw-bold py-2">All the latest news</h2>
        <hr class="my-0 mx-auto" />
      </div>
      <div class="row mt-5">
        <div
          v-for="(item, index) in latestNewsProps"
          :key="index"
          class="col-4"
        >
          <a href="#">
            <img class="img-fluid" :src="`/img${item.img}`" alt="" />
          </a>
          <div class="fw-bold pt-1">{{ item.title }}</div>
          <div class="subtitle pt-1">
            <span> {{ item.subtitle }} </span>
            <strong> {{ item.comments }}</strong>
            <p class="py-2">{{ item.paragraph }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    latestNewsProps: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/rowItemsStyle.scss";
</style>
