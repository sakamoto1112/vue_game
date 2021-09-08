<template>
  <div class="alert alert-info">
    <h2>{{ title }}</h2>
    <h3>{{ message }}</h3>
    <!-- <p>{{ comment }}</p> -->
  </div>
</template>

<script>
export default {
  name: 'Question',
  props: {
    title: String,
    message: String,
    // comment: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h2 {
  margin: 20px 0 0;
  color: crimson;
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
