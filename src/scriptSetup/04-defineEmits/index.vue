<template>
  {{count}}
  <infoTs @parentClick="parentClick" @parentChange="parentChange"></infoTs>
</template>

<script lang="ts" setup>
import infoTs from "./info-ts.vue";
import {ref} from "vue";
const count = ref(1)
const parentClick = (data:number) =>{
  alert('子组件触发了父组件的 parentClick')
  count.value +=data
}
const parentChange = () =>{
  alert('子组件触发了父组件的 parentChange')
}
</script>

<style scoped>

</style>
