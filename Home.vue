<template>
<h1>Home Component{{ 10+10 }}</h1>
<h1>Home Component{{ 'hello'.length }}</h1>
<h1>Email:{{ email }}</h1>
<h1>Mobile:{{ mobile }}</h1>
<h1>Mobile:{{ mobile==7535051925 }}</h1>
<h1>Name:{{ getName() }}</h1>

</template>

<script>
export default {
    name: 'Home',
    data () {
        return {
        email:'bharat123tiwari123@gmail.com',
        mobile: 9389591306,
        getName: function() {
            return "Bharat Tiwari"
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
