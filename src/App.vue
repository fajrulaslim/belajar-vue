<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <hr>
  <C01DataDanMethods />
  <hr>
  <C02DataBinding />
  <hr>
  <C03TwoWayDataBinding />
  <hr>
  <C04ConditionalDanLoops />
  <hr>
  <C05LifecycleDanHooks />
  <hr>
  <C06ComputedProperties />
  <hr>
  <C07ComponentsDanProps :text="text" />
  <hr>
  <C08CustomEvents @sendTxt="terimaText" />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import C01DataDanMethods from './components/C01DataDanMethods.vue'
import C02DataBinding from './components/C02DataBinding.vue'
import C03TwoWayDataBinding from './components/C03TwoWayDataBinding.vue'
import C04ConditionalDanLoops from './components/C04ConditionalDanLoops.vue'
import C05LifecycleDanHooks from './components/C05LifecycleDanHooks.vue'
import C06ComputedProperties from './components/C06ComputedProperties.vue'
import C07ComponentsDanProps from './components/C07ComponentsDanProps.vue'
import C08CustomEvents from './components/C08CustomEvents.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    C01DataDanMethods,
    C02DataBinding,
    C03TwoWayDataBinding,
    C04ConditionalDanLoops,
    C05LifecycleDanHooks,
    C06ComputedProperties,
    C07ComponentsDanProps,
    C08CustomEvents,
  },
  data() {
    return {
      text: "Kirim Props dari App dengan data binding"
    }
  },
  methods: {
    terimaText(txt) {
      this.text = txt
    }
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
