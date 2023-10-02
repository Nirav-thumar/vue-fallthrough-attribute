<template>
    <h1>hello</h1>
</template>
 
 
<script setup>
 
import { ref, reactive, computed  } from 'vue'
 import {useAttrs} from 'vue'

 const attrs = useAttrs();
 console.log(attrs);
</script>
 
<style scoped>
 
</style>