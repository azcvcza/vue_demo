<template>
  <div class="bind">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'bind',
  data : () => {
    return {
      msg : 'to use router',
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bind{
    background-color:#58a;
}
</style>
