<template>
    <div id="app">
        <h1>子から親への値渡し</h1>
        <HelloWorld :title="message" @result-event="appAction"></HelloWorld>
        <hr>
        <p>{{result}}</p>
    </div>
</template>

<script>
import HelloWorld from './components/3_4.vue'

export default {
    name:'App',
    components:{
        HelloWorld
    },
    data() {
        return {
            message:'Hello',
            result:''
        }
    },
    methods: {
        appAction(message){
            this.result="(you send '"+message+"' )"
        }
    },
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
