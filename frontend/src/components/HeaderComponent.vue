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
  height: 25vw;
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
    font-size: 5vw;
  }

  h2 {
    font-size: 4vw;
  }

  h3 {
    font-size: 3vw;
  }

  h4 {
    font-size: 2vw;
  }
}

.logo-sized {
  min-width: 75%;
  width: 75%;
  align-self: center;
}

.flex-center {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
