<template>
  <div id="menuContainer">
      <ul>
          <li v-for="item in menu" v-bind:key="item.id">
              {{item.name}}
          </li>
      </ul>
  </div>
</template>

<script>
export default {
    props: ['menu'],
    data() {
        return {
            
        }
    }
}
</script>

<style>
#menuContainer {
    padding-right: 50px;
    border-right: 1px solid #cdcdcd;
}
</style>