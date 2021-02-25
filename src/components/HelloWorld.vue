<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      We know naming things are hard, but Phil is here to help! Just type what you're working on and see what Phil would name your project.
      
    </p>
    <input type="text" v-model="input" />
    
    <h3>Your project name is:</h3>
    
    <p v-show="input != ''">{{input}} of Netlify</p>
  </div>

  
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      input:''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
