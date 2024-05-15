<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <hr>
  <C01DataDanMethods />
  <hr>
  <C02DataBinding />
  <hr>
  <C03TwoWayDataBinding />
  <hr>
  <C04ConditionalDanLoops />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import C01DataDanMethods from './components/C01DataDanMethods.vue'
import C02DataBinding from './components/C02DataBinding.vue'
import C03TwoWayDataBinding from './components/C03TwoWayDataBinding.vue'
import C04ConditionalDanLoops from './components/C04ConditionalDanLoops.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    C01DataDanMethods,
    C02DataBinding,
    C03TwoWayDataBinding,
    C04ConditionalDanLoops,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
