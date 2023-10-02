<template>

<!-- Attribute inheritance in root element of component -->
 <!-- <Child class="btn-pink" id="childId" style="background-color:blue;color:white" @click="btnClick"/>
 <div  style="background-color:red;color:green">check</div>
 <div>{{count}}</div> -->

<!-- merging -->
  <!-- <Child  class="btn-pink" id="parent" style="color:red;border:1px solid red;" @click="eventpfParent()"/> -->


<!-- attribute inheritance in nested component with merging -->
<!-- <Child class="btn-parent" id="parentId" style="background-color:green" @click="btnClick"/> -->

<!-- disabling attribute -->
<DisableInheritance class="btn-pink" id="parent" style="border:1px solid red;" :style="{color:red}" @click="eventpfParent()" />


<!-- attribute inheritance in multiple root element -->
 <!-- <MultipleRoot class="parentClass" id="parentId" style="background-color:blue;color:white" @click="btnClick"/> -->

<!-- useAttrs()  in script setup-->
 <!-- <useAttrs class="parentClass" id="parentId" style="background-color:blue;" :style="{color:red}" @click="btnClick"/> -->

</template>

 
 
<script setup>
 
import { ref, reactive, computed  } from 'vue'
import Child from './Child.vue'
import DisableInheritance from './DisableInheritance.vue'
import MultipleRoot from './MultipleRoot.vue'
import UseAttrs from './UseAttrs.vue'


 const red = ref('red');
 const green =ref('green');
 const count =ref(0)

 function btnClick(){
  console.log('button is clisked from child')
  count.value++;

 }

 function eventpfParent(){
  console.log('eventofParent')
 }

 setTimeout(()=>{
  red.value = "green"
  console.log('green')
 },2000)
</script>
 
<style scoped>
 
</style>