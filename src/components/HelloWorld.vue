<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <v-btn @click="setacessToken(true)">enable access</v-btn>
    <v-btn @click="setacessToken(false)">disable access</v-btn>

  </div>
</template>

<script>
import {mapActions} from 'vuex'

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods:{
     ...mapActions([
      'setacessToken'
      ])
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
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
