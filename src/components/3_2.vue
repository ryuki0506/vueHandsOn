<template>
    <div>
        <h2>{{title}}</h2>
        <p>{{message}}</p>
        <hr>
        <div>
            <input type="text" v-model='input'>
            <button @click="doAction">Click</button>
        </div>
    </div>
</template>

<script>
export default {
    name:'HelloWorld',
    props:{
        title:String,
    },
    data() {
        return {
            message:'お名前は？',
            input:'',
        }
    },
    methods: {
        doAction(){
            this.message='Hello '+this.input+'!'
        }
    },
}
</script>