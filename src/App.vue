<template>
  <div id="app">
    <h2>Input a text</h2>
      <input type="text" v-model="inp"/>
           <button @click="tocapital()">submit</button>
    <div id="preview">
      <h3>Preview of the text in UpperCase letters</h3>
      <p>Uppercase Letter: {{capital}}</p>
    </div>
  </div>
</template>

<script>

export default 
{
  data(){
    return{
        inp: "",
        capital: ""} },
        methods:{
        tocapital:function (){
        this.capital=this.inp.toUpperCase();
      }   }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
