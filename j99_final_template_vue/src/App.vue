<template>
  <div id="app">
    <HeaderMain/>
    <NavMobile />
    <!-- router-view représente toutes les routes de premiers niveaux -->
    <router-view/>
    <FooterMain/>
  </div>
</template>
<script>
import HeaderMain from "@/views/partials/Header.vue";
import NavMobile from "@/views/partials/NavMobile.vue";
import FooterMain from "@/views/partials/Footer.vue";
export default {
  components: {
    HeaderMain,
    FooterMain,
    NavMobile
  }
};
</script>

<style lang="scss">
* {
  margin: 0;
  box-sizing: border-box;
}

a {
  text-decoration: none;
}

.page {
  top: 120px;
  position: relative;
  min-height: calc(100vh - (120px + 200px));
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  & > * {
    padding: 10px 20px;
  }
  position: relative;
}
</style>
