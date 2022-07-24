<script lang="ts" setup>
//import
import { ref } from "@vue/reactivity";

let isShow = ref(false);
</script>

<template>
  <header>
    <!-- Container -->
    <div class="container">
      <!-- responsive sidebar main -->
      <nav class="main" v-show="isShow == true">
        <!-- Svg -->
        <svg
          @click="isShow = !isShow"
          class="close-menu"
          xmlns="http://www.w3.org/2000/svg"
          width="15"
          height="15"
          viewBox="0 0 24 24"
        >
          <path
            d="M24 20.188l-8.315-8.209 8.2-8.282-3.697-3.697-8.212 8.318-8.31-8.203-3.666 3.666 8.321 8.24-8.206 8.313 3.666 3.666 8.237-8.318 8.285 8.203z"
          />
        </svg>
        <a href="#">Collections</a>
        <a href="#">Men</a>
        <a href="#">Women</a>
        <a href="#">About</a>
        <a href="#">Concat</a>
      </nav>

      <!-- Hamburger and logo  -->
      <div class="hamburger-btn" @click="isShow = !isShow">
        <svg
          class="open-menu"
          v-show="isShow == false"
          viewBox="0 0 100 80"
          width="25"
          height="25"
        >
          <rect width="100" height="20"></rect>
          <rect y="30" width="100" height="20"></rect>
          <rect y="60" width="100" height="20"></rect>
        </svg>
      </div>
      <div class="logo">
        <img
          v-show="isShow == false"
          style="margin-left: 3px"
          alt="Sneaker-logo"
          src="../assets/HeaderSvg/logo.svg"
        />
      </div>

      <!-- Main list  -->
      <nav class="mains">
        <a href="#">Collections</a>
        <a href="#">Men</a>
        <a href="#">Women</a>
        <a href="#">About</a>
        <a href="#">Concat</a>
      </nav>

      <!-- Baskket and user  -->
      <nav class="basket-user">
        <img class="basket" src="../assets/HeaderSvg/basket.svg" alt="" />
        <img class="avatar" src="../assets/HeaderSvg/image-avatar.png" alt="" />
      </nav>
    </div>
  </header>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  height: 100px;
  // container
  .container {
    border-bottom: 1px solid #e8eef1;
    display: flex;
  }
  //mains
  .mains {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    height: 100px;
    a {
      font-size: 17px;
      color: rgb(104, 112, 125);
      margin-left: 35px;
    }
  }
  // hamburger btn
  .hamburger-btn {
    display: none;
    justify-content: flex-start;
    align-items: center;
    height: 100px;
    svg {
      display: flex;
      cursor: pointer;
    }
  }
  // logo
  .logo {
    display: flex !important;
    align-items: center;
    justify-content: flex-start;
    height: 100px;
    img{
      margin-left: 15px !important;
    }
  }

  .basket-user {
    width: 100%;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: flex-end !important;
    .basket {
      margin-right: 25px;
      cursor: pointer;
    }
    //profil photo 
    .avatar {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      cursor: pointer;
    }
  }
}
// responsive
@media only screen and (max-width: 900px) {
  .hamburger-btn {
    display: flex !important;
  }
  .main {
    display: flex;
    width: 150px !important;
    flex-direction: column !important;
    align-items: flex-start !important;
    height: 100vh !important;
    background: white !important;
    border-right: 1px solid #f1f1f1;
    padding: 0px 10px;
    box-sizing: border-box;
    z-index: 10;

    a {
      margin-top: 15px !important;
      font-weight: bold;
      color: rgb(29, 32, 37) !important;
      margin-right: 20px;
    }
    svg {
      margin-top: 15px;
      margin-right: 15px;
      cursor: pointer;
    }
  }
  .mains {
    display: none !important;
  }
}
</style>
