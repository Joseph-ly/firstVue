<template>
  <div id="app" class="container">
    <!-- <router-view/> -->
    <div id="componentWrapper" class="d-flex justify-content-start">
      <hello></hello>
      <menuList v-bind:menu="menuList"></menuList>
    </div>
    <formArea></formArea>
  </div>
</template>

<script>
  import Nihao from './components/Hello';
  import menuList from './components/Menu';
  import formArea from './components/formArea';

  export default {
    name: 'app',
    components: { 
      hello: Nihao,
      menuList,
      formArea,
    },
    data() {
      return {
        menuList: [
          {id: 1, name: 'Dashboard'},
          {id: 2, name: 'Notification'},
          {id: 3, name: 'Universe'},
          {id: 4, name: 'Setting'},
        ]
      }
    }
  }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
