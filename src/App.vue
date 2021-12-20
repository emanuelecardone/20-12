<template>
  <div id="app">
    <NewTitle />
    <SassTitle />
    <MixinsPart />
  </div>
</template>

<script>
import NewTitle from "./components/NewTitle.vue";
import SassTitle from "./components/SassTitle.vue";
import MixinsPart from "./components/MixinsPart.vue";

export default {
  name: "App",
  components: {
    NewTitle,
    SassTitle,
    MixinsPart
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  width: 100%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
