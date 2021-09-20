<template>
    <div id="app">
        <h1>プロジェクトを作る</h1>
        <HelloWorld title="Hello" message="This is a sample page."></HelloWorld>
    </div>
</template>

<script>
import HelloWorld from './components/3_2.vue'

export default {
    name:'App',
    components:{
        HelloWorld
    }
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
