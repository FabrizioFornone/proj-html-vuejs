<template>
  <section>
    <div class="container">
      <div class="row py-3">
        <div
          v-for="(item, index) in latestNews2Props"
          :key="index"
          class="col-4"
        >
          <a href="#">
            <img class="img-fluid" :src="`/img${item.img}`" alt="" />
          </a>
          <div class="fw-bold pt-1">
            {{ item.title }}
          </div>
          <div class="subtitle pt-1">
            <span> {{ item.subtitle }} </span>
            <strong>{{ item.comments }}</strong>
            <p class="py-2">
              {{ item.paragraph }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    latestNews2Props: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/rowItemsStyle.scss";
</style>
