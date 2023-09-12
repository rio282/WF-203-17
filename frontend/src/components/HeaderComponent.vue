<template>
  <div class="header bg-dark row">
    <div class="left-brand col">
      <img class="float-start logo-sized" src="../assets/images/test.png" alt="brand 1">
    </div>

    <div class="mid-section col flex-center">
      <div class="">
        <h1 class="text-primary">Electric Scooter Rental</h1>
        <h3 class="text-dark-emphasis">
          By:
          <a class="text-dark-emphasis" href="https://www.example.com" target="_blank">Rio</a>
          &
          <a class="text-dark-emphasis" href="https://www.example.com" target="_blank">Kingsley</a>
        </h3>
      </div>
    </div>

    <div class="right-brand col">
      <img class="float-end logo-sized" src="../assets/images/test.png" alt="brand 2">
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent"
}
</script>

<style scoped>
.header {
  height: 30em;
  width: 100%;
  overflow: hidden;
  margin-bottom: 0.5em;
}

div > * {
  color: white;
}

.mid-section {
  text-align: center;
  align-content: center;
  align-items: center;
  justify-content: center;
  justify-items: center;
}

  h1 {
    font-size: 5em;
  }

  h2 {
    font-size: 4em;
  }

  h3 {
    font-size: 3em;
  }

  h4 {
    font-size: 2em;
  }



.logo-sized {
  min-width: 5rem;
  width: 30rem;
  align-self: center;
}

.flex-center {
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>
