<template>
  <div class="alert alert-info">
    <h2>{{ title }}</h2>
    <h3>{{ message }}</h3>
    <hr>
    <div>
      <!-- <input class="form-control" type="text" v-model="input"> -->
      <button class="btn-info mt-2" v-on:click="doAction">
      Click</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Answer',
  props: {
    title: String,
    message: String,    
  },

  data() {
    return {
      seikai:"正解！",
      fuseikai:"不正解。。。"
    };
  },
  
  methods: {
    doAction() {
      if(this.message === "北岳") {
        console.log("正解")
      } else {
        console.log("不正解")
      }
      // if(this.answer === "北岳") {
      //   this.message = "正解！";
      // } else {
      //   this.message = "不正解！";
      // }
      
    }
  },
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
