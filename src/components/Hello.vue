<template>
  <div id="hello">
      <!-- <img src="../assets/logo.png"> -->
      <h1>{{msg}}</h1>
      <h2>This is: {{name}}</h2>
      <h3>Date: {{nowDate}}</h3>
      <button class="btn btn-primary" @click="countClickTimes">Clicked Times: {{times}}</button>
  </div>
</template>

<script>
export default {
    name: 'NiHao',
    data() {
        return {
            msg: 'Hello World.',
            name: 'Joseph',
            times: 0,
        }
    },
    methods: {
        countClickTimes: function() {
            this.times++
        }
    },
    computed: {
        nowDate: function() {
            return new Date().toLocaleString();
        }
    },
}
</script>

<style>
#hello {
    border-right: 1px solid #cdcdcd;
    padding-right: 50px;
}
</style>