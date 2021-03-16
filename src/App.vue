<template>
<div id="app">
<CompHeader/>
  <list-user v-bind:listUser="listUser" />
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <comp-footer/>
</div>
  

</template>

<script>
import CompFooter from './components/CompFooter.vue';
import CompHeader from './components/CompHeader.vue';
import ListUser from './components/ListUser.vue';
export default {
  name: 'App',
 data (){
   return {
     listUser:[
       {
         id:1 , name:'cong'
       },
         {
         id:2 , name:'congg'
       },
         {
         id:3 , name:'conggg'
       },
     ]
   }
 },
  components: {
    CompHeader,
    CompFooter,
    ListUser,
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
