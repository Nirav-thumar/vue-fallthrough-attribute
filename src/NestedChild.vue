<template>
 
 <!-- attribute nested component -->    
  <button class="btn-nestedchild" id="nestedchildId" style="background-color:blue;color:blue" @click="eventofNestedChild">buttonclick</button>
</template>
 
 
<script setup>
 
import { ref, reactive, computed  } from 'vue'
 
 function eventofNestedChild(){
  console.log('nested component called')
 }
</script>
 
<style scoped>
 
</style>