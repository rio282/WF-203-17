<template>
  <div class="header bg-dark row">
    <div class="left-brand col">
      <img class="rounded float-start w-75" src="../assets/test.png" alt="brand 1">
    </div>

    <div class="mid-section col">
      <h1 class="text-primary">Electric Scooter Rental</h1>
      <h3 class="text-dark-emphasis">
        By:
        <a class="text-dark-emphasis" href="https://www.example.com" target="_blank">Rio</a>
        &
        <a class="text-dark-emphasis" href="https://www.example.com" target="_blank">Kingsley</a>
      </h3>
    </div>

    <div class="right-brand col">
      <img class="rounded float-end w-75" src="../assets/test.png" alt="brand 2">
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

  h1 {
    font-size: 60px;
  }

  h2 {
    font-size: 40px;
  }

  h3 {
    font-size: 30px;
  }

  h4 {
    font-size: 20px;
  }
}
</style>
