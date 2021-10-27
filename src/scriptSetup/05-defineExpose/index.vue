<template>
  <info-setup ref="InfoRef"></info-setup>
</template>

<script lang="ts" setup>
import InfoSetup from './info-setup.vue'
import {onMounted, ref} from "vue";
const InfoRef = ref(null)

onMounted(() =>{
  console.log(InfoRef.value,InfoRef.value.count)
  InfoRef.value.handle()
})
</script>

<style scoped>

</style>
