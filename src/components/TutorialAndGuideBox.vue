<template>
  <section>
    <div class="container py-4">
      <div class="row">
        <div class="col-8 bg-dark">
          <div>
            <h5 class="text-uppercase">rewiewed article</h5>
            <h1>
              Mauris viverra atisan ipsum eget felis primis efficitur varius
            </h1>
            <p class="py-2">
              In quis lectus sed leo elementum faucibus in dapibus dictum.
              Nullamolestie tortor nec lectus venenantis, sed landit, dui, dolor
              at bibendum sadips ets ipsum dolores ficilis uns leo lectus
            </p>
            <button class="text-uppercase fw-bold my-2 px-5 py-2 rounded btn">
              <a href="#"></a>read more
              <i class="fas fa-angle-right px-1"></i>
            </button>
          </div>
        </div>
        <div class="col-4">
          <div class="ps-3">
            <h3 class="fw-bold py-2">Tutorials & Guides</h3>
            <hr />
            <div
              v-for="(item, index) in tutorialAndGuideProps"
              :key="index"
              class="d-flex py-3"
            >
              <a href="#">
                <img :src="`/img${item.img}`" alt="" />
              </a>
              <div class="px-2">
                <div class="fw-bold">
                  {{ item.title }}
                </div>
                <div class="subtitle py-1">
                  <span> {{ item.subtitle }} </span>
                  <span>{{ item.comments }}</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    tutorialAndGuideProps: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/fifthSectionStyle.scss";
</style>
