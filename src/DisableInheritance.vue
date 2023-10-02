<template>
<button class="btn-pink" id="parent" style="color:green;border:1px solid green" @click="eventodDisable()" >
 click </button>
 <div class="main">
    <!-- <div v-bind="$attrs" id="disabled-id" class="disabled-class" style="color:white;background-color:green;border:2px solid blue" @click="eventodDisable()">fallthrougn</div> -->
   
   <!-- to check attrs change will take or not if changes donw from parent -yes -->
    <!-- <div v-bind="$attrs" id="disabled-id" class="disabled-class"  @click="eventodDisable()">fallthrougn</div> -->
 </div>
</template>
 
 
<script setup>
 
import { ref, reactive, computed  } from 'vue'
 
 function eventodDisable(){
    // console.log('disabled event called');
    console.log('fallthorough')
 }
</script>

<script>
export default{
    inheritAttrs:false
}

</script>

 
<style scoped>
 
</style>

