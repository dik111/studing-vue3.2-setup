<template>
  <DefinePropsRuntime title="DefinePropsRuntime" :list="list"></DefinePropsRuntime>
</template>

<script lang="ts" setup>
import DefinePropsRuntime from "./defineProps-runtime.vue";
const list = [
  {id:1,content:'1'},
  {id:2,content:'2'}
]
</script>

<style scoped lang="less">

</style>
