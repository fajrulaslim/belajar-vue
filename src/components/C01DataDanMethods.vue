<template>
    <div>
        Hello {{ nama }}, Selamat Datang di Vue.js
    </div>
    <button @click="changeName">Change Name</button> <button v-on:click="resetName">Reset Name</button>
</template>

<script>
export default {
  name: 'C01DataDanMethods',
  data() {
    return {
      nama: "Fajrul Aslim",
    }
  },
  methods: {
    changeName() {
      this.nama = "Fajrul Aslim"
    },
    resetName() {
      this.nama = "World"
    }
  }
}
</script>