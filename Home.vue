<template>
<h1>Email: {{ email }}</h1>
<h1>Name: {{ getName() }}</h1>
<h1>Name: {{ getNick("Bhanu") }}</h1>
<h1>Name 2: {{ getNick("Alisha") }}</h1>
<h1>All Data:{{ getData() }}</h1>
<h1>All Data: {{ getData().name }}</h1>
<h1>All Data: {{ getData().email }}</h1>

</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            email: 'bharat123tiwari123@gmail.com'
        }
    },
    methods:{
        getName() {
            return "Bharat Tiwari"
        },
        getNick(name){
            return name;
        },
        getData() {
            return {
                name:"Akhil",
                email:"akhil@gmail.com",
               // email:this.email

            }
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
