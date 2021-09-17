<template>
  <div class="hello">
    <h1>{{ text }}</h1>
    <img alt="Vue logo" src="../assets/logo.png">
    <p>This is Vue page</p>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    text: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>