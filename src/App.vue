<template>
  <div id="app">
    <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand href="#">Account Management</b-navbar-brand>

        </b-navbar>
   
    <Create @add-text="addText1"/>
    <Tablelist v-bind:items="items"/>

   
  </div>
  
</template>

<script>

import Create from './components/Create'
import Tablelist from './components/Tablelist'
export default {
  name: 'app',
  components:{
    Create,Tablelist
  },
  methods:{
    addText1(text1){
      this.items.push(text1);
    }
  }
}
</script>

<style>
</style>
