<template>
  <button @click="handleClick">Click</button>
</template>

<script lang="ts">
export default {
  name: 'App',
  methods: {
    handleClick(e:any){
      console.log(e)
      if (gtag) {
        gtag('send', 'button_click')
      }
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
