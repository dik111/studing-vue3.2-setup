<template>
  <button @click="handleClick">点击触发 handleClick事件，并且传递2给父组件</button>
  <div>
    点击触发 handleChange 事件 <input type="checkbox" name="" @change="handleChange"/>
  </div>
</template>

<script lang="ts" setup>
import {defineEmits} from "vue";

const emit =  defineEmits<{
  (e:'parentClick',data:number):void,
  (e:'parentChange'):void,
}>()
const handleClick = () =>{
  emit("parentClick",2)
}
const handleChange = () =>{
  emit("parentChange")
}
</script>

<style scoped>

</style>
