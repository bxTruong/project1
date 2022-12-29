<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <header-app ref="header"/>
  <MyModal
    v-if="isShowModal" 
    title="This is new title from App" 
    content="This is new content form App" 
    theme="sale"
    @cancel="onToggleShowModal"
    >
    <template v-slot:header></template>
  <label for="">Name</label>
  <input type="password" >
  </MyModal>
  <button @click="onToggleShowModal">Show modal</button>
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
    onToggleShowModal(){
      this.isShowModal =!this.isShowModal;
    }
  },
  data(){
    return {
    isShowModal : false,
    }
  }
}
</script>

<style></style>

