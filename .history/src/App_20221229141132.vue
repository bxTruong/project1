<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <header-app ref="header"/>
  <MyModal/>
  <button @click="onChange">Change me</button>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue';
import MyModal from './components/MyModal.vue';
import './components/MyModal.vue';

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

