<template>
  <div class="hello">
    <h2>{{ title }}</h2>
    <span>{{ msg }}</span>
  </div>
</template>

<script>

export default {
  name: 'Thanks',
  state () {

  },
  data () {
    return {
      title: '鍵開け依頼フォーム',
      msg: '送信完了しました。'
    }
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
