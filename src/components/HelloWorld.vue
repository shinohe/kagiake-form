<template>
  <div class="hello">
    <h2>{{ title }}</h2>
    <span>{{ msg }}</span>
    <div class="frame">
      <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSd54xM2RgBeuaAismlZmR4RBDWaWUbeMJ31IulwwSud_zNwUg/viewform?embedded=true" frameborder="0" marginheight="0" marginwidth="0">読み込んでいます…</iframe>
    </div>
      
  </div>
</template>

<script>

export default {
  name: 'KagiAkeForm',
  data () {
    return {
      title: '鍵開け依頼フォーム',
      msg: '※イベント外でも好みであれば開けます',
      shareName: '',
      twitterId: '',
      description: ''
    }
  },
  methods: {
    send () {
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

.frame{
    position:relative;
    width:100%;
    height:0;
    padding-top:220%;
}
.frame iframe{
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
}
</style>
