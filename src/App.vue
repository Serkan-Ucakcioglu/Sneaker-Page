<script lang="ts" setup>
//import
import HeaderBar from "./components/HeaderBar.vue";
import SectionContent from "./components/SectionContent.vue";
</script>
<template>
  <!-- Components -->
  <HeaderBar />
  <SectionContent />
  <!-- Components -->
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Kumbh+Sans&display=swap");
#app {
  font-family: "Kumbh Sans", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-weight: 700;
}
a {
  text-decoration: none;
}

.container {
  width: 90%;
  max-width: 1250px;
  margin: 0px auto;
}
</style>
