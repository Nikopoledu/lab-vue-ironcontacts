<script setup>
import contacts from "./contacts.json";
import HelloWorld from './components/HelloWorld.vue'

const myContacts = contacts;
console.log(myContacts)
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <table v-for="contact in myContacts" v-bind:key="contact">
    <td><img  :src="contact.pictureUrl" style="width:60px;" alt=""></td>
    <td>{{ contact.name}}</td>
    <td>{{ contact.popularity}}</td>
    
   
    
    
    </table>
  <HelloWorld msg="Hello Vue 3 + Vite" />
</template>

<style>
#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font: Helvetica sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

table {
   width: 100%;
}
th, td {
   width: 25%;
   text-align: center;
   vertical-align: top;
}
</style>
