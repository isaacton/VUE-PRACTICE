<template>
    <p>firstName</p>

    <input type="text" v-model="firstName">

    <p>lastName</p>

    <input type="text" v-model="lastName">


<p>{{ firstName }} {{ lastName }}</p>


    <h1 v-if="NUMBER === 100">THE NUMBER IS 100</h1>
    <h1 v-else-if="NUMBER > 100">THE NUMBER IS GREATER THAN 100</h1>
    <h1 v-else-if="NUMBER < 100">THE NUMBER IS LESS THAN 100</h1>
    <h1 v-else>THE number is not 100</h1>
    <p :title="message">hen</p>
    <h1 v-if="showText">This is my personal components and i love it so much yeah.</h1>
    <h1 v-else>ISAAC</h1>
    <h1>{{ 2 + 30 }}</h1>
    <h1>{{name}}</h1>
    <p v-html="school"></p>
    <h1>{{ok?"Present":"absent"}}</h1>
    <button v-bind:disabled="btnDisable">click  me</button>
    
    <button v-on:click="display">Toggle button</button>
<p v-html="hack"></p>
</template>


<script>
export default {
    name: 'MyPersonalComponent',
    data() {
        return{
            name: 'isaac',
            age: 45,
            school: '<b>IMT</b>',
            ok: true,
            btnDisable: true,
            message: "STRONGEST",
            showText: true,
            NUMBER: 99,
            hack: '<a href="#">www.google.com</a>',
            firstName: "",
            lastName: ""
        }
    },
    methods: {
        le(){
            // this.isaac = "james"
            this.name = "shame"
        },
        head(){
            this.ok = !this.ok
        },
        display(){
            this.showText = !this.showText
        }
    }
}
</script>

<style>
h1{
    background-color: dodgerblue;
    color: white;
}
p{
    color: green;
}
</style>