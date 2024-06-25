<script setup>
import { reactive } from 'vue'
const inisial = reactive({ val: { jumlah: 0 }, user: ['aku', 'dia'] })
const gantiUser = () => {
  inisial.user[0] = 'kamu'
  inisial.user[1] = 'anda'
}
</script>

<template>
  <h1>namanya {{ inisial.val.jumlah }}</h1>
  <h1>namanya {{ inisial.user }}</h1>
  <button @click="inisial.val.jumlah += 1">add 1</button>
  <button @click="gantiUser">user</button>
  <button>tambah lagi</button>
</template>
