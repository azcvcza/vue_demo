<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <input type="text" v-model="message">
    <button v-on:click="console">click me to log</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data : () => {
    return {
      msg : 'Welcome to Your Vue.js App',
      message : 'input your answer'
    }
  },
  methods:{
    console : function () {
      console.log('button click')
    }
  },
  init: function () {
    console.log('init');
  },
  created: function () {
    console.log('created');
  },
  beforeCompile: function () {
    console.log('before complied')
  },
  compiled: function () {
    console.log('complied')
  },
  attached: function () {
    console.log('attached')
  },
  dettached: function () {
    console.log('dettached')
  },
  beforeDestroyed: function () {
    console.log('beforeDestroyed')
  },
  destroyed: function () {
    console.log('destroyed')
  },
  ready: function ()　{
    console.log('ready');
    this.$destroy();
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
