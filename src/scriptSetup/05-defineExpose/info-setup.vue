<template>
{{count}}
</template>

<script lang="ts">
export default {

}
</script>
<script lang="ts" setup>
import {ref} from 'vue'

const count = ref(2)

const handle = () =>{
  console.log('这是子组件的方法')
}

// defineExpose({
//   count,handle
// })

</script>

<style scoped>

</style>
