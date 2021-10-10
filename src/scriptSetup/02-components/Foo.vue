<template>
  <h1>Foo</h1>
  {{count}}
  <button @click="add">+1</button>
</template>

<script lang="ts" setup>

import {ref} from "vue";

const count = ref(1);
const add = () =>{
  count.value ++;
}
</script>

<style scoped>

</style>
