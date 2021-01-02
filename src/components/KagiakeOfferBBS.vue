<template>
  <div class="hello">
    <h2>{{ title }}</h2>
    <span>{{ msg }}</span>
    <Ads></Ads>
    <div class="contents">
    </div>
    <Ads></Ads>
      
  </div>
</template>

<script>

export default {
  name: 'KagiAkeForm',
  data () {
    return {
      title: '鍵開け依頼板',
      msg: '誰かが開けてくれるかもしれない板'
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


@media only screen and (max-width: 600px) {
  .frame{
    position:relative;
    width:100%;
    height:0;
    padding-top:840px;
  }

}

</style>
