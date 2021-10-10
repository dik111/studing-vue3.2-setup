<template>
  <h1>DefinePropsRuntime</h1>
  <p>{{title}}</p>
  <ul>
    <li v-for="item in list " :key="item.id">{{item.content}}</li>
  </ul>
</template>

<script lang="ts" setup>
import {defineProps} from "vue";

defineProps({
  title:{
    type:String,
    required:true
  },
  list:{
    type:Array,
    required:true
  }
})
</script>

<style scoped>

</style>
