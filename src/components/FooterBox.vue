<template>
  <footer>
    <div class="container">
      <div class="d-flex py-5">
        <div class="col-3">
          <div class="px-2">
            <div class="fs-5 fw-bold text-uppercase py-3">avada tech forum</div>
            <p>
              Sed semper, nisl id feugiat eleifend, erat est digssim felis, quis
              auctor elit enim nec ante. Cras et nibh risus. pellentesque non mi
              sit amet mi intermentum
            </p>
          </div>
        </div>
        <div v-for="(item, index) in footerProps" :key="index" class="col-3">
          <div class="px-2">
            <div class="fs-5 fw-bold text-uppercase py-3">{{ item.title }}</div>
            <ul>
              <li>
                <a href="#">{{ item.item1 }}</a>
              </li>
              <li>
                <a href="#">{{ item.item2 }}</a>
              </li>
              <li>
                <a href="#">{{ item.item3 }}</a>
              </li>
              <li>
                <a href="#">
                  {{ item.item4 }}
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <hr id="footer-hr" />
    <div class="container my-5">
      <div class="d-flex justify-content-between">
        <div class="end-line">
          <span class="copyright-span">Copiright 2012 -2020</span>
          <span>|</span>
          <span
            >Avada <strong> <a href="#">Theme Fusion</a> </strong></span
          >
          <span>|</span> <span>All Righjts Reserved</span><span>|</span>
          <span
            >Powered by <strong> <a href="#">WordPress</a> </strong>
          </span>
        </div>
        <div class="d-flex icon-box">
          <a href="#">
            <i id="facebook-icon" class="fab fa-facebook-f rounded-circle"></i>
          </a>
          <a href="#">
            <i id="twitter-icon" class="fab fa-twitter rounded-circle"></i>
          </a>
          <a href="#">
            <i id="instagram-icon" class="fab fa-instagram rounded-circle"></i>
          </a>
          <a href="#">
            <i id="youtube-icon" class="fab fa-youtube rounded-circle"></i>
          </a>
        </div>
      </div>
    </div>
    <div class="fixed-bottom d-flex justify-content-end">
      <a @click="scrollUp()" href="#">
        <i class="fas fa-chevron-up mx-5 px-3 py-2 rounded end-chevron"></i>
      </a>
    </div>
  </footer>
</template>

<script>
export default {
  props: {
    footerProps: Array,
  },
  methods: {
    scrollUp() {
      window.scrollTo(0, 0);
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/footerStyle.scss";
</style>
