<template>
  <header>
      <div class="list-user">
          <!-- <p>List user component</p>
           -->
           <user v-for="user in listUser"
           v-bind:key="user.id"
           v-bind:user="user"/>
          
      </div>
  </header>
</template>

<script>
import User from './User.vue';
export default {
  name: 'list-user',
  props:{
      listUser:{
          type : Array,
          default:function(){
            return [];
          }
          // default : [],
      }
  },
  data(){
    return {
      
    }
  },
  components :{
      User,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
