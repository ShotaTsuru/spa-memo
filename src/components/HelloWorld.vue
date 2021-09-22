<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2 v-show="showText">{{ test }}</h2>
    <button v-on:click="toggle">toggle</button> <!--追加!!!!!!-->
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      test: 'test vue',
      showText: false
    }
  },
  methods: {
    toggle: function () {
      this.showText = !this.showText
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
</style>
