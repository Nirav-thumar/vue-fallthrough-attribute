<template>
   <!-- Attribute inheritance in root element of component -->

    <!-- <button>click</button> -->

    <!-- merging -->
    <!-- <button class="btn" id="child" style="color:green;background-color:gray" @click="eventofChild()">click</button> -->

  <NestedChild class="btn-child" id="childId" style="background-color:red;color:red" @click="eventofChild"/>

</template>
 
 
<script setup>
 
import { ref, reactive, computed  } from 'vue'
import NestedChild from './NestedChild.vue'
 
 function  eventofChild(){
    console.log('eventofchild');
 }
</script>
 
<style scoped>
 
</style>