<template>
    <div>
      <input type="text" v-model="email"> <br>
      {{ email }}
    </div>
</template>
  
<script>
export default {
    name: 'C03TwoWayDataBinding',
    data() {
        return {
            email: "",
        }
    }
}
</script>