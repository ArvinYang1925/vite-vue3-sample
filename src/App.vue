<script setup>
import { ref } from 'vue'

// i. 定義值
const num = ref(1) // 使用 ref 定義響應式的狀態 num，初始值為 1

// ii. 針對值要做的事情
function clickMe() {
  num.value++
}
</script>

<template>
  {{ num }}

  <button v-on:click="clickMe">Click</button>
</template>
