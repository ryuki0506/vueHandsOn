<template>
  <div>
    <h1>{{ title }}</h1>
          <button @click="doAction">
        Click
      </button>
    <p ref="msg">{{ message }}</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      title:'Hello World',
      message:'this is sample massage.',
    }
  },
  mounted() {
    this.counter=0
  },
  methods: {
    doAction(){
      this.counter++
      this.$refs.msg.innerHTML+='<h6>counted:'+this.counter+'</h6>'
    }
  },
}
</script>