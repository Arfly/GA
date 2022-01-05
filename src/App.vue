<template>
  <button @click="handleClick">Click</button>
</template>

<script lang="ts">
export default {
  name: 'App',
  methods: {
    handleClick(e:any){
      console.log(e)
      if (ga) {
        ga('send', 'button_click')
      }
    }
  }
}

function ga(arg0: string, arg1: string) {
throw new Error("Function not implemented.")
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
