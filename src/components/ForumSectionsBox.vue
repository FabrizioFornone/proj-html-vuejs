<template>
  <section>
    <div class="banner py-4 mt-3 d-flex justify-content-center">
      <div class="text-uppercase fw-bold my-5">
        <a href="#"
          >read our blog
          <i class="fas fa-long-arrow-alt-right px-1"></i>
        </a>
      </div>
    </div>
    <div class="container-fluid">
      <div class="container">
        <div class="text-center pt-5">
          <h5 class="text-uppercase">phasellus eget metus</h5>
          <h2 class="fw-bold py-2">Forum Sections</h2>
          <hr class="my-0 mx-auto" />
        </div>
        <div class="row py-5">
          <div
            v-for="(icon, index) in iconsProps"
            :key="index"
            class="col-3 mt-4"
          >
            <a href="#">
              <div class="d-flex flex-column align-items-center p-5 icon-box">
                <i
                  :class="`${icon.family} ${icon.prefix}${icon.name} d-flex align-items-center justify-content-center rounded-circle`"
                ></i>
                <div class="fw-bold pt-2">News & community</div>
              </div>
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="banner py-4 mt-3 d-flex justify-content-center">
      <div class="text-uppercase fw-bold my-5">
        <a href="#"
          >Go to our forum
          <i class="fas fa-long-arrow-alt-right px-1"></i>
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    iconsProps: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/sixthSectionStyle.scss";
</style>
