<template>
  {{count}}
  <button @click="add">+1</button>
</template>

<script lang="ts">
import {defineComponent, ref} from 'vue'

export default defineComponent({
  setup(){
    const count = ref(2)
    const add = () =>{
      count.value ++;
    }
    return {
      count,
      add
    }
  }
})
</script>

<style scoped>

</style>
