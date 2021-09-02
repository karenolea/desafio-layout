<template>
  <v-app>
    <Navbar></Navbar>
    <Card
      
      
    ></Card>

    
  </v-app>
</template>

<script>
import Navbar from './components/Navbar';
import Card from './components/Card';

export default {
  name: 'App',


  components: {
    Navbar,
    Card
   
  },
 
  
};
</script>
