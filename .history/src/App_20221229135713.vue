<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld ref="hello" msg="Welcome to Your Vue.js App"/>
  <header-app ref="header"/>
  <MyModal/>
  <button @click="onChange">Change me</button>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue';
import MyModal from './components/MyModal.vue';

export default {
  name: 'App',
  components: {
    HeaderApp: HeaderApp,
    MyModal,
  },
  methods:{
    onChange(){
      console.log(this.$refs.hello);
      console.log(this.$refs.header);
      this.$refs.hello.onConsoleTesting();
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
