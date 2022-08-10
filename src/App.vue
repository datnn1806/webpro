<template>
  <div id="app">
    <p v-show="show">mất hết</p>
    <p>{{name}}</p>
    <button @click="show = !show">click</button>
    <br>
    <input type="text" name="" id="" v-model="name">
    <div v-if="showClassName">fullstack</div>
    <div v-else >caimeosgifthe</div>
    <input type="checkbox" v-model="showClassName" name="" id="">
    <HelloDat/>
    <Menu/>
  </div>
</template>

<script>
import HelloDat from "./components/HelloDat.vue";
import Menu from "./components/Menu.vue";


export default {
  data() {
    return {
      showClassName:false,
      show:false,
      name:'nguyen thanh dat'
    }
  },
  name: 'App',
  components: {
    HelloDat,
    Menu
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
