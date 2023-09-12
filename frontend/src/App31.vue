<template>
  <HeaderComponent></HeaderComponent>
  <NavBar></NavBar>
  <WelcomeComponent></WelcomeComponent>
  <link rel="stylesheet" href="node_modules/bootstrap/dist/css/bootstrap.css"/>

</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import NavBar from "@/components/NavBar";
import WelcomeComponent from "./components/WelcomeComponent.vue";


export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "App31",
  components: {
    HeaderComponent,
    WelcomeComponent,
    NavBar

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
