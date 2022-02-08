<template>
  <header class="fixed-top">
    <div class="container">
      <div class="d-flex justify-content-between align-items-center py-2">
        <div>
          <img class="logo" src="@/assets/img/logo-2x.png" alt="" />
        </div>
        <nav>
          <ul class="d-flex align-items-center">
            <li><a href="#">Home</a></li>
            <li><a href="#">Apple</a></li>
            <li><a href="#">Microsoft</a></li>
            <li><a href="#">Android</a></li>
            <li><a href="#">Forums</a></li>
            <li><a href="#">Contact us</a></li>
            <li>
              <button class="text-uppercase rounded"><a href="#">join us</a></button>
            </li>

            <li>
              <i
                id="lens"
                class="fas fa-search"
              ></i>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/style/headerStyle.scss";
</style>
