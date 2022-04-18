<template>
<GenerateQuote />  
  <generator/>
</template>

<script>
import GenerateQuote from './GenerateQuote.vue'

export default {
  components: {
    GenerateQuote
    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #f9fafb;
  margin-top: 60px;

}
  body{
  background-image: url('./assets/road.jpg');

}

</style>
