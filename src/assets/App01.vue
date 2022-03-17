<script setup>
import contacts from "./contacts.json";
import HelloWorld from './components/HelloWorld.vue'

const myContacts = contacts;
console.log(myContacts)
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <div v-for="contact in myContacts">{{ contact.name}}</div>
  <HelloWorld msg="Hello Vue 3 + Vite" />
</template>

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
