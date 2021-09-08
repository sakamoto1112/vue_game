<template>
  <div id="app">
    
    <Question v-bind:title="mondai" />
      <!-- title="問題文"
      message="日本で二番目に高い山は？" /> -->
    <Answer
      title="解答Ａ"
      v-bind:message="kotae.A" />
    <Answer
      title="解答Ｂ"
      v-bind:message="kotae.B" />
    <Answer
      title="解答Ｃ"
      v-bind:message="kotae.C" />
    <Answer
      title="解答Ｄ"
      v-bind:message="kotae.D" />
    
  </div>
</template>

<script>
import Question from "./components/Qustion.vue";
import Answer from "./components/Answer.vue";

export default {
  name: "App",
  components: {
    Question,
    Answer,
  },
  data() {
    return {
      mondai: "日本で二番目に高い山は？",
      kotae: {
        A:"北岳",
        B:"奥穂高岳",
        C:"劔岳",
        D:"立山"
      }
    }
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}
</style>
