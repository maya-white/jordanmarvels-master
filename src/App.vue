<template>
  <div id="app">
    <div id="nav">
      <top-header></top-header>
    </div>
    <router-view />
    <footer>
      <top-footer></top-footer>
      <bottom-footer></bottom-footer>
    </footer>
  </div>
</template>

<script>
import TopHeader from "./components/common/TopHeader.vue";
import TopFooter from "./components/common/TopFooter";
import BottomFooter from "./components/common/BottomFooter";
export default {
  components: {
    "top-header": TopHeader,
    "top-footer": TopFooter,
    "bottom-footer": BottomFooter
  }
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.heading {
  color: #50473d;
  font-weight: bold;
  position: relative;
  margin-bottom: 20px;
  &::before {
    content: "";
    position: absolute;
    width: 100px;
    border-top: 2px solid #d5d5d5;
    top: 50%;
    left: -125px;
  }
}
section {
  padding-top: 50px;
}
</style>
