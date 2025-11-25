<template>
<h1 v-on:mousemove="getConsole()">Home Component</h1>
<button v-on:click="getData()">Click me</button>
<button v-on:click="getData('Button 2 Clicked')">Click me</button>
<button v-on:dblclick="getData('Button double Clicked')">Click me</button>
<h2>{{ count }}</h2>

</template>

<script>
export default {
    name: 'Home',
    data () {
        return  {
            count:0
        }
    },
    methods: {
        getData() {
            this.count=this.count+1;
        },
        getConsole() {
            console.log("function called")
        }
    }
   
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>