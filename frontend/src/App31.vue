<template>
  <HeaderComponent></HeaderComponent>
  <WelcomeComponent></WelcomeComponent>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import WelcomeComponent from "./components/WelcomeComponent.vue";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "App31",
  components: {
    HeaderComponent,
    WelcomeComponent
  }
}
</script>

<style scoped>
  * {
    box-sizing: border-box;
  }

  body {
    font-family: Arial, Helvetica, sans-serif;
    margin: 0;
  }
</style>
