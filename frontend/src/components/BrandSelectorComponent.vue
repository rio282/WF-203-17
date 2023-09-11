<template>
  <div class="bsc col-auto col-md-3 bg-dark">
    <div class="d-flex flex-column align-items-center align-items-md-start text-white min-vh-100">
      <h3>Pick a brand:</h3>
      <div class="btn-group">
        <button class="btn btn-secondary btn-md dropdown-toggle" id="_button" type="button" data-bs-toggle="dropdown"
                aria-expanded="false">
          Select a brand...
        </button>
        <ul class="dropdown-menu">
          <li v-for="brand in brands" :key="brand.name" @click="doSomethingWithBrand(brand)">
            <a class="dropdown-item" href="#">{{ brand.name }}</a>
          </li>
        </ul>
      </div>

      <h3>Availability</h3>
      <ul class="">
        <li v-for="place in places" :key="place.count" @click="doSomethingWithPlace(place)">
          <a class="" href="#">{{ place.name }}&nbsp;-&nbsp;{{ place.count }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "BrandSelectorComponent",
  data() {
    return {
      selectedBrand: null,
      brands: [
        {
          "name": "a"
        },
        {
          "name": "b"
        },
        {
          "name": "c"
        },
      ],
      places: [
        {
          "name": "amsterdam",
          "count": this.rnd(),
        },
        {
          "name": "utrecht",
          "count": this.rnd(),
        },
        {
          "name": "leiden",
          "count": this.rnd(),
        },
      ]
    }
  },
  methods: {
    rnd() {
      const min = 10
      const max = 50;
      return Math.floor(Math.random() * (max - min) + min);
    },

    doSomethingWithBrand(brand) {
      this.selectedBrand = brand;
      document.getElementById("_button").innerHTML = brand.name;
      console.log(`selected brand: ${brand.name}`)
    },

    doSomethingWithPlace(place) {
      console.log(`selected place: ${place.name} (${place.count})`)
    },
  }
}
</script>

<style scoped>
.bsc {
  margin-right: 0.5em;
}
</style>