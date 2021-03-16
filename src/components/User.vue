<template>
  <header>
   <div class="user">
       <p>{{user.name}}</p>
   </div>
  </header>
</template>

<script>
export default {
  name: 'user',
  props:{
    user:{
      type: Object,
      default: null
    }
  },
  data(){
    return {
        
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
