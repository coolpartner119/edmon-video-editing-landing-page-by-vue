<script>

import { RouterLink, RouterView } from 'vue-router'

export default {

  data() {
    return {
      showMobileMenu: false,
    };
  },
  methods: {
    showMenu() {
      this.showMobileMenu = !this.showMobileMenu;
    },
  },
};
</script>

<template>
  <div>
    <div class="line_header " :class="this.showMobileMenu ? 'active' : ''"></div>
    <RouterLink to="/about" class="mobile access-btn">Request Beta Access</RouterLink>
    <div class="spinner-master" :class="this.showMobileMenu ? 'active' : ''">
      <div id="spinner-form" className="spinner-spin" @click="showMenu()">
        <div className="spinner diagonal part-1"></div>
        <div className="spinner horizontal"></div>
        <div className="spinner diagonal part-2"></div>
      </div>

      <div id="mobileMenu" class="mobileMenu" :class="this.showMobileMenu ? 'active' : ''" @click="showMenu()">
        <ul class="responsivemenu">
          <li>
            <RouterLink to="/" class="project-btn">Product</RouterLink>
          </li>
          <li><a href="https://edmon-test.web.app/" class="about-btn">Sign in</a></li>
        </ul>
      </div>
    </div>
  </div>

</template>

<style   scoped>
/* Responsive */
#mobileMenu {
  display: none;
}

.line_header {
  display: none;
  width: 100%;
  height: 1px;
  position: fixed;
  top: 64px;
  left: 0;
  z-index: 9999;
  background-color: #f5f5f594;
}

.line_header.active {
  display: flex;
}

@media(max-width: 1200px) {
  .spinner-spin {
    width: 24px;
    height: 24px;
  }

  .spinner-form {
    display: block;
  }

  .spinner-master * {
    -webkit-transition: all 0.3s;
    transition: all 0.3s;
    box-sizing: border-box;
    flex-wrap: wrap;
    z-index: 999;
  }

  .spinner-master {
    width: 50px;
    position: relative;
    display: flex;
    align-items: center;
    background: transparent;
    height: 46px;
    z-index: 9990;
  }

  /* .spinner:nth-child(2n) {
    width: 70% !important
  } */

  .spinner-master label {
    cursor: pointer;
    height: auto;
    width: 100%;
    padding: 0;
    -webkit-transform: translateY(0%);
    transform: translateY(0%);
    top: -13px;
    position: relative;
  }

  .spinner-master .spinner {
    height: 2px;
    width: 100%;
    background-color: #ffffff;
  }

  .spinner-master.active .spinner-spin>.horizontal {
    opacity: 0;
    -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
  }

  .spinner-master.active .spinner-spin>.diagonal.part-1 {
    transform: rotate(135deg);
    -webkit-transform: rotate(135deg);
    margin-top: 9px;
  }

  .spinner-master.active .spinner-spin>.diagonal.part-2 {
    transform: rotate(-135deg);
    -webkit-transform: rotate(-135deg);
    margin-top: -20px;
  }


  #mobileMenu {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 99;
    overflow: hidden;
    background-color: rgba(13, 13, 24, .7);
    --nav-saturate: 150%;
    -webkit-transition: all 0.4s ease 10s;
    transition: all 0.4s ease 10s;
    font-weight: 600;
    font-size: 24px;
    line-height: 127.19%;
    /* identical to box height, or 31px */

    text-align: right;
    letter-spacing: 0.035em;
  }

  #mobileMenu.active {
    max-height: 100em;
    overflow: auto;
    width: 100%;
    height: 210px;
    background: rgba(58, 62, 97, 0.84);
    backdrop-filter: blur(4px);
    position: fixed;
    display: flex;
    justify-content: flex-end;
    padding-right: 16px;
    font-weight: 600;
    font-size: 24px;
    box-shadow: inset 0px -0.5px 0px rgba(255, 255, 255, 0.25);
    border-radius: 0px 0px 0px 72px;
    flex-direction: row;
  }

  #mobileMenu>ul ul.show {
    display: flex;
    flex-direction: r;
  }

  #mobileMenu>ul>li {
    display: block !important;
  }



  #mobileMenu>ul>li:last-child>a {
    border-bottom: 0px
  }

  #mobileMenu li.has-submenu>a:before,
  .mainmenu ul>li.active a:before {
    display: none;
  }

  .megamenu.active {
    padding: 15px 0 !important
  }

  .sub-menu:before {
    height: 90% !important;
    left: 50% !important;
    -webkit-transform: translate(-50%, -50%) !important;
    transform: translate(-50%, -50%) !important;
  }

  .sub-menu:after {
    display: none
  }

  .responsivemenu :first-child {
    margin-top: 36px;
    margin-bottom: 16px;
  }

  #mobileMenu li.has-submenu>a.active:after {
    content: "-";
  }

  #mobileMenu ul ul>li a {
    padding: 7px 20px;
    font-size: 16px;
    color: #fff
  }

  #mobileMenu ul ul>li a,
  #mobileMenu ul ul>li p {
    padding: 10px 20px;
    line-height: normal;
    -webkit-text-fill-color: #fff;
    display: block;
  }

  .mainmenu ul li ul li {
    border: none
  }


  #mobileMenu p {
    margin: 0;
    line-height: normal;
  }

}
</style>