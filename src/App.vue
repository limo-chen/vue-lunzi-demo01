<template>
<router-view />
</template>

<script lang="ts">
import{ref,provide}from 'vue'

export default {
  name: 'App',
  setup(){
    const witch =document.documentElement.clientWidth
    const menuVisible = ref(witch <= 300 ? false :true)
    provide('menuVisible',menuVisible)
    
  }
}
</script>
