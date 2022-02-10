<template>
  <section>
    <div class="banner mt-3 d-flex justify-content-center">
      <button class="text-uppercase fw-bold my-4 px-5 py-2 rounded">
        <a href="#"
          >read our blog
          <i class="fas fa-long-arrow-alt-right px-1"></i>
        </a>
      </button>
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
              <div class="text-center p-5 icon-box">
                <i
                  :class="`${icon.family} ${icon.prefix}${icon.name} rounded-circle`"
                ></i>
                <div class="fw-bold pt-2">News & community</div>
              </div>
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="banner mt-3 d-flex justify-content-center">
      <button class="text-uppercase fw-bold my-4 px-5 py-2 rounded">
        <a href="#"
          >Go to our forum
          <i class="fas fa-long-arrow-alt-right px-1"></i>
        </a>
      </button>
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
