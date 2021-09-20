<template>
    <div id="app">
        <h1>親から子への値渡し</h1>
        <HelloWorld :title="message"></HelloWorld>
        <hr>
        <button @click="doAction">Change title</button>
    </div>
</template>

<script>
import HelloWorld from './components/3_3.vue'

export default {
    name:'App',
    components:{
        HelloWorld
    },
    data() {
        return {
            message:'Hello'
        }
    },
    methods: {
        doAction(){
            this.message=prompt("new title:")
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
