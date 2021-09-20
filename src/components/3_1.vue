<template>
    <div>
        <h2>{{title}}</h2>
        <p>{{message}}</p>
    </div>
</template>

<script>
export default {
    name:'HelloWorld',
    props:{
        title:String,
        message:String,
    }
}
</script>