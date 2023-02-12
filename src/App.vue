
<script >
import { RouterLink, RouterView } from 'vue-router'
import mobileMenu from './views/mobileMenu.vue';
export default {
  name: "app",
  components: {
    mobileMenu,
  },
  data() {
    return {
      limitPosition: 500,
      scrolled: false,
      lastPosition: 0
    };
  },

  methods: {
    handleScroll() {

      if (this.lastPosition < window.scrollY && this.limitPosition < window.scrollY) {
        this.scrolled = true;
        // move up!
      }

      if (this.lastPosition > window.scrollY) {
        this.scrolled = false;
        // move down
      }

      this.lastPosition = window.scrollY;
    }
  },
  created() {
    window.addEventListener("scroll", this.handleScroll);
  },
  destroyed() {
    window.removeEventListener("scroll", this.handleScroll);
  }
};
</script>

<template>
  <header :class="{ 'headroom--unpinned': scrolled }" v-on="handleScroll" class="headroom header">
    <div class="max-w-1440">
      <img alt="Vue logo" class="logo" src="@/assets/logo.png" />
      <mobileMenu />
      <div class="wrapper">
        <nav>
          <RouterLink to="/" class="project-btn">Product</RouterLink>
          <a href="https://edmon-test.web.app/" class="about-btn">Sign in</a>
          <RouterLink to="/about" class="access-btn">Request Beta Access</RouterLink>
        </nav>
      </div>
    </div>
  </header> 
  <RouterView />

  <footer>
    ©2023 EdMon.AI | All rights reserved.
    <div>
      <a href="">
        <img src="./assets/images/footer/mdi_instagram.png" alt="" srcset="">
      </a>
      <a href="">
        <img src="./assets/images/footer/ic_baseline-facebook.png" alt="" srcset="">
      </a>
    </div>

  </footer>
</template>


<style scoped>
.mobile {
  display: none;
}

@media (max-width: 1200px) {
  .mobile {
    display: block;
    width: 50px;
    height: 50px;
    position: absolute;
    top: 10px;
    right: 10px;
  }
  .wrapper .access-btn {
    display: none;
  }
}
</style>
