<script setup>
import { ref } from 'vue'
const benar = true
const salah = false
let raguRagu = ref(true)
</script>

<template>
  <p v-if="salah">ini yang salah</p>
  <p v-else-if="benar">ini yang benar</p>
  <p v-else>tidak keduanya ? maybe?</p>
  <p v-show="raguRagu">ini yang pake shownya</p>
  <button @click="raguRagu = !raguRagu">ini ngetest lawan dari ragu ragu nya</button>
</template>
