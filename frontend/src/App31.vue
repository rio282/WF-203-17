<template>
  <HeaderComponent></HeaderComponent>

  <div class="row">
    <BrandSelectorComponent></BrandSelectorComponent>
    <WelcomeComponent></WelcomeComponent>
    <InformationComponent></InformationComponent>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import WelcomeComponent from "./components/WelcomeComponent.vue";
import BrandSelectorComponent from "@/components/BrandSelectorComponent.vue";
import InformationComponent from "@/components/InformationComponent.vue";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "App31",
  components: {
    InformationComponent,
    BrandSelectorComponent,
    HeaderComponent,
    WelcomeComponent
  }
}
</script>

<style scoped>
  * {
    box-sizing: border-box;
    scroll-behavior: smooth;
  }

  body {
    font-family: Arial, Helvetica, sans-serif;
    margin: 0;
    background: red;
  }
</style>
