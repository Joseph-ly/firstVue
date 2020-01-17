<template>
  <div id="menuContainer">
      <ul>
          <li v-for="item in menu" v-bind:key="item.id" v-bind:style="styleObject">
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
            styleObject: {
                listStyle: 'none'
            }
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