<script lang="ts" setup>
import HeaderBar from './components/HeaderBar.vue';
import SectionContent from './components/SectionContent.vue';
</script>
<template>
  <HeaderBar msg="Welcome to Your Vue.js + TypeScript App"/>
  <SectionContent/>
</template>



<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
a{
  text-decoration: none;
}


.container{
  width: 90%;
  max-width: 1250px;
  margin: 0px auto;
}

</style>
