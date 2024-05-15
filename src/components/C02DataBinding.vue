<template>
  <a :href="web" target="_blank">Website</a> | <a v-bind:href="github" target="_blank">Github</a>
</template>

<script>
export default {
  name: 'C02DataBinding',
  data() {
    return {
      web: "https://fajrulaslim.com",
      github: "https://github.com/fajrulaslim",
    }
  }
}
</script>